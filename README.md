**🚢 Kaggle Titanic — Machine Learning from Disaster**
Kaggle 排名：**TOP 3,979** / 150,000+ 参赛者

本仓库包含我在 Kaggle “Titanic: Machine Learning from Disaster” 比赛中的完整解决方案，包括数据清洗、基本特征工程、多模型比较与最终预测提交。

**📌 1. 项目背景（Project Background）**

本项目的任务是预测泰坦尼克号乘客是否获救，这是一个经典的二元分类问题。
项目主要考察：

数据清洗与缺失值处理
特征预处理与编码
多模型训练与对比
生成可提交的预测结果

**📌 2. 我的解决方案（My Approach）**

以下流程完全基于本项目 Notebook 的真实步骤：

**① 数据加载**

使用 train.csv 和 test.csv 作为输入数据

查看数据维度与基本结构

**② 数据清洗（Data Cleaning）**

你在 Notebook 中做了：

Age 缺失值填充中位数

Embarked 缺失值填充众数

清理 Ticket、Cabin 等列

对不需要的特征进行删除（如 PassengerId 在训练中未使用）

**③ 特征编码（Feature Encoding）**

**Label Encoding**
对 Sex、Embarked 和 Cabin 的类别值进行整数编码

**④ 模型训练与比较（Modeling）**

训练并比较了以下模型：

Logistic Regression

Support Vector Machine (SVC)

RandomForestClassifier

AdaBoostClassifier

GradientBoostingClassifier

比较指标：Accuracy（在训练集上）

Notebook 输出了模型表现对比，选出最好的模型。

**⑤ 最终模型（Final Model: RandomForestClassifier ）**

选择了表现最好的模型，并用它生成提交文件：

submission.csv

上传到 Kaggle 得到了 3979 名 的成绩。

**📌 3. Kaggle 成绩（Kaggle Ranking）**
项目	排名	参赛人数
Titanic: Machine Learning from Disaster	**3,979 名**	150,000+

**📌 4. 文件结构（Repository Structure）**
├── README.md                     
├── Titanic Classification.ipynb      
├── train.csv / test.csv              
├── submission.csv                   
├── assets/
│   └── kaggle_score.png              

**📌 5. 环境要求（Environment Requirements）**
python 3.8+
pandas
numpy
matplotlib
seaborn
scikit-learn

**📌 6. 如何运行（How to Run）**

下载本仓库

打开 Notebook：Titanic Classification.ipynb

运行所有单元格

会自动生成 submission.csv

上传到 Kaggle 查看分数

**📌 7. 项目亮点（Key Highlights）**

全流程机器学习分类项目
数据清洗与 Label Encoding 简洁明了
使用多种模型进行对比
最终排名进入 Kaggle 前 3%–4%
Notebook 结构清晰，易于复现
