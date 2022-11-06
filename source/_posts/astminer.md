title: astminer的jar包命令行调用
date: 2022-11-06 23:52:09
categories: astminer

tags: astminer
---
astminer-0.6的jar包在方法级上生成code2vec数据格式
<!-- more -->

astminer：[JetBrains-Research/astminer: A library for mining of path-based representations of code (and more) (github.com)](https://github.com/JetBrains-Research/astminer)

### 参考链接

1.[(24条消息) 用astminer生成code2vec输入数据格式的方法_蛐蛐蛐的博客-CSDN博客](https://blog.csdn.net/qysh123/article/details/106309967)
2.https://blog.csdn.net/lockhou/article/details/113854491

### 实验代码
在jar包目录下打开终端，本文用的0.6版本，其具体格式如下：

`java -jar lib-0.5.jar code2vec --lang cpp --project %源代码的目录% --output %需要生成的code2vec的输入数据的目录%`

使用示例如下，此外该方法可对单个文件或整个文件夹进行处理。

`java -jar lib-0.6.jar code2vec --lang java --project D:/test/Contra_Learning/samesemantic2/convert/333433_1_convert_0.java --output D:/test/Contra_Learning/test`

其中，lib-0.6.jar为当前目录下的jar包，code2vec表示输出格式(preprocess, parse, pathContexts, code2vec), --lang用于配置语言，可用-h或者是--help命令来查看不同输出格式下的参数配置信息。

`java -jar lib-0.6.jar code2vec -h`

### 问题总结

在运行该命令行语句时,发现方法级文件所生成的结果文件中除path_contexts文件外均为空，尝试对源文件加入public class test{}后再运行上述指令，运行结果正常。因此可暂且采用此方法在方法级上生成code2vec数据格式。

### 结果分析
node_types.csv包含数字ID和带有方向的相应节点类型（如纸张所述，向上/向下）可理解为箭头朝向。
tokens.csv 包含数字ID和相应的标记。
paths.csv 以空格分隔的节点类型ID序列形式包含数字ID和全部的AST路径，其中AST路径中的数字对应node_types文件中的数字ID。
path_contexts.csv 包含路径上下文的标签和序列（两个标记的三元组以及它们之间的路径）。该三元组分别包含了两个终端节点及他们之间的路径，三元组中的路径的数字对应paths文件中的ID。
如果使用code2vec格式的副本，则每行path_contexts.csv以一个标签开头，然后它包含一系列以空格分隔的三元组。每个三元组包含开始令牌ID，路径ID，结束令牌ID，以逗号分隔。
如果使用csv格式，则其中的每一行都path_contexts.csv包含标签，然后是逗号，然后是-;分隔的三元组序列。每个三元组包含开始令牌ID，路径ID，结束令牌ID，以空格分隔。

