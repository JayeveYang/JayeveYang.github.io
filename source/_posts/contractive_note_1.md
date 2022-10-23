title: 对比学习学习笔记（一）
date: 2022-10-22 23:30:09
categories: 对比学习
tags: Contrastive Learning
相关工作及论文<<基于图嵌入的代码相似性度量>>（梁瑶、谢春丽等著）学习
<!-- more -->
---
### 对比学习相关论文：
1.《Efficient Framework for Learning Code Representations through Semantic-Preserving Program Transformations》
2.《Contrastive Code Representation Learning》
3.《HELoC: Hierarchical Contrastive Learning of Source Code Representation》
### 目前工作相关论文：
1.《基于图嵌入的代码相似性度量》
2.《Code Clone Detection based on Contrastive Learning》

### 相关工具：
1.等价语义转换：JavaTransformer / tnpa-generalizability-master
2.方法级代码块抽取：JavaMethodExtractor
3.多种表示形式抽取工具：astminer（token，ast，path，path contexts）

### 现有实验代码：
1.graph_embedding:基于图嵌入的代码相似性度量
2.clone_detection:基于对比学习的代码克隆检测（token级别）
### 数据说明：
Category 已对原始bcb数据级进行扩展后的方法级代码数据
---
# 基于图嵌入的代码相似性度量