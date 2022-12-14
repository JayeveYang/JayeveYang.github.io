title: 对比学习相关材料
date: 2022-10-22 23:30:09
categories: 对比学习
tags: Contrastive Learning
---
对比学习相关工作
<!-- more -->
### 相关论文
1.《Efficient Framework for Learning Code Representations through Semantic-Preserving Program Transformations》
2.《Contrastive Code Representation Learning》
3.《HELoC: Hierarchical Contrastive Learning of Source Code Representation》

### 目前工作相关论文
1.《基于图嵌入的代码相似性度量》
2.《Code Clone Detection based on Contrastive Learning》

### 相关工具
1.等价语义转换：JavaTransformer / tnpa-generalizability-master
2.方法级代码块抽取：JavaMethodExtractor
3.多种表示形式抽取工具：astminer（token，ast，path，path contexts）

### 现有实验代码
1.graph_embedding:基于图嵌入的代码相似性度量
2.clone_detection:基于对比学习的代码克隆检测（token级别）

### 数据说明
Category 已对原始bcb数据级进行扩展后的方法级代码数据

### 相关链接
1.Contrastive Self-Supervised Learning-Ankesh Anand
https://ankeshanand.com/blog/2020/01/26/contrative-self-supervised-learning.html
2.小全读论文《Momentum Contrast for Unsupervised Visual Representation Learning》
https://blog.csdn.net/FatMigo/article/details/103211622?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522163845153216780357248122%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=163845153216780357248122&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~hot_rank-1-103211622.first_rank_v2_pc_rank_v29&utm_term=Momentum+Contrast+for+Unsupervised+Visual+Representation+Learning&spm=1018.2226.3001.4187
3.对比学习1
https://mp.weixin.qq.com/s/EOlXjdd1gCruiF-B1JoIgg
4.更好的对比样本选择，更好的对比效果
https://mp.weixin.qq.com/s?__biz=MzIwMTc4ODE0Mw==&mid=2247539589&idx=2&sn=4525c7cbb3aa3e0534f048574c6f125f&scene=21#wechat_redirect
5.理解对比表示学习(Contrastive Learning)
https://blog.csdn.net/xxxxxxxxxx13/article/details/110820373?spm=1001.2101.3001.6650.1&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7Edefault-1.no_search_link&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7Edefault-1.no_search_link
6.用astminer生成code2vec输入数据格式的方法
https://blog.csdn.net/qysh123/article/details/106309967
7.code2vec的初步应用
https://blog.csdn.net/lockhou/article/details/113854491?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522164442824016780255216752%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=164442824016780255216752&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-2-113854491.first_rank_v2_pc_rank_v29&utm_term=%E7%94%A8astminer%E7%94%9F%E6%88%90code2vec%E8%BE%93%E5%85%A5%E6%95%B0%E6%8D%AE%E6%A0%BC%E5%BC%8F%E7%9A%84%E6%96%B9%E6%B3%95&spm=1018.2226.3001.4187
8.对比学习（Contrastive Learning）中的损失函数
https://blog.csdn.net/yyhaohaoxuexi/article/details/113824125?spm=1001.2101.3001.6650.13&utm_medium=distribute.pc_relevant.none-task-blog-2~default~BlogCommendFromBaidu~Rate-13-113824125-blog-111478798.pc_relevant_antiscanv2&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2~default~BlogCommendFromBaidu~Rate-13-113824125-blog-111478798.pc_relevant_antiscanv2&utm_relevant_index=15