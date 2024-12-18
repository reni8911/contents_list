## repositories 目录
---
### 一、AIDD
----------------
#### 1. 靶点研究
- **项目：单细胞转录组**
- 描述：根据不同癌种高分文献，搭建的标准分析SOP，包括原始数据定量，细胞注释，细分亚型，不同亚型在不同组织中的差异基因、功能注释等。以及用于药物治疗前后临床前研究的个性化分析。
- 用途：研究靶点表达、作用机制、适应症等
- **github**: https://github.com/reni8911/scRNA-seq

#### 2. 分子生成
- **项目：非天然氨基酸分子生成**
- 描述：基于非天然氨基酸的骨架，使用LSTM+self-attentionmo组合模型, 训练prior模型以修饰骨架，然后利用强化学习，根据分子性质(SA、 RF、 MW等) 优化模型，最终生成复合目标性质的非天然氨基酸库。
- 任务：生成+强化学习
- 用途：用于RDC药物的binder(线性、环状肽)生成，通过排列组合非天然氨基酸。
- **github**: 
  - https://github.com/reni8911/UAA_DB
  - https://github.com/reni8911/scaffold-dataset
  - https://github.com/reni8911/scaffold-modification



#### 3. 分子筛选
- **项目：ADMET 预测**
- 描述：基于TDC公开数据库，使用多种编码器，编码药物，结合神经网络模型，对药物的分布、代谢、排泄等多种分子性质进行预测。
- 模型选择与优化：15种以上的编码器，覆盖从经典的化学信息学指纹，到深度神经网络(MLP)、卷积神经网络(CNN)、变换器(Transformer)以及消息传递图神经网络(MPNN)的广阔范围，结合深度学习模型。分别训练并调优，选择top10的模型集成。
- 任务：分类、回归
- 用途：用于RDC药物初步筛选

- **github**
  - https://github.com/reni8911/ADMET_prediction
  - https://github.com/reni8911/RTlogD74
  
  
- **项目：DTA 预测**
- 描述：基于TDC公开数据库，使用多种编码器，分别编码药物和靶点，结合神经网络模型，预测药物靶点的亲和力。
- 模型选择与优化：15种以上的编码器，覆盖从经典的化学信息学指纹，到深度神经网络(MLP)、卷积神经网络(CNN)、变换器(Transformer)以及消息传递图神经网络(MPNN)的广阔范围，结合深度学习模型。分别训练并调优，选择top10的模型集成。
- 任务：回归
- 用途：识别与特定靶点具有高亲和力的药物。
- **github**
  - https://github.com/reni8911/DTA_prediction
  - https://github.com/reni8911/pepPI_pred    
<br>



### 二、科研文章
---
#### 1. 统计模型
- 描述：基于癌症患者的影像、临床病理特征，使用Logistic 模型、KM 生存分析、Cox 生存分析等方法，分析参数与预后的关系。
- **github**: https://github.com/reni8911/statistical_model

#### 2. 机器学习
- 描述：基于癌症患者的影像、临床病理特征，使用特征筛选、传统机器学习方法，预测癌症分级、预后结局等。
- 任务：分类
- **github**: https://github.com/reni8911/ML

#### 3. 深度学习
- 描述：基于前列腺癌患者的多序列MR影像，使用convmixer模型，并优化，预测良恶性、临床显著的良恶性。
- 任务：分类
- **github**: https://github.com/reni8911/PCa_MR_classification_train

<br>

### 三、医学影像
---
#### 1. 传统图像算法
- MR_multiseq_regist：前列腺癌MR多序列配准
  - github：https://github.com/reni8911/MR_multiseq_regist

- trad_body_seg：人体分割
  - github：https://github.com/reni8911/trad_body_seg
  

#### 2. AI图像算法
- Pca_MR_classification：前列腺癌良恶性预测
  - github: https://github.com/reni8911/Pca_MR_classification
- body_seg：人体分割
  - github：https://github.com/reni8911/body_seg

<br>

### 四、软著
---
- MR_DataManager：MR图像管理系统
  - github: https://github.com/reni8911/MR_DataManager
- UAA_DB：非天然氨基酸数据库
  - github: https://github.com/reni8911/UAA_DB
- ADMET_prediction：ADMET预测
  - github：https://github.com/reni8911/ADMET_prediction
- LogD74_prediction: LogD74预测
  - github：https://github.com/reni8911/RTlogD
- DTA_prediction：DTA预测
  - github：https://github.com/reni8911/DTA_prediction
- pepPI_pred：多肽-蛋白质相互作用预测
  - github：https://github.com/reni8911/pepPI_pred
