Chem-KD: Multi-View Knowledge Distillation Framework for Data-Scarce Chemical Learning

Chem-KD_Tg:主体全部数据与代码
Chem-KD_Tg/database:模型所使用数据（data-set）、提取的图数据特征（gragh-feature）、训练完成的模型参数（model）以及软标签数据（soft-label）
Chem-KD_Tg/feature_extractor：p-SMILES转图特征数据代码（包括含标签以及不含标签的特征提取代码）
Chem-KD_Tg/trainer：模型训练代码包含教师模型、Chem-KD模型以及基础模型训练代码
Chem-KD_Tg/predictor：基于输入的已转换特征的p-SMILES进行预测的代码

Chem-KD_Tg与Chem-KD_DC(+freq)为同结构文件夹，Chem-KD_DC(+freq)代码包含新加入的全局特征freq表征介电常数的测试频率

prediction of literature data and experimental data：实验合成结构的p-SMILES转的图数据特征以及最优模型预测结果

本库可使用Chem-KD_XX中的feature_extractor和predictor，通过调用最优参数，对需要的p-SMILES进行Tg或者DC进行预测


Hard requirements
These packages must be available to use Chem-KD:
"""python
python=3.9.23=h716150d_0
deepchem=2.8.0=pypi_0
rdkit=2024.3.5=pypi_0
torch=2.3.1+cu118=pypi_0
torch-geometric=2.6.1=pypi_0
torch-scatter=2.1.2+pt23cu118=pypi_0
torch-sparse=0.6.18+pt23cu118=pypi_0
torch-cluster=1.6.3+pt23cu118=pypi_0
torch-spline-conv=1.2.2+pt23cu118=pypi_0
numpy=1.26.3=pypi_0
pandas=2.3.3=pypi_0
scikit-learn=1.6.1=pypi_0
scipy=1.13.1=pypi_0
matplotlib=3.9.4=pypi_0
joblib=1.5.2=pypi_0
tqdm=4.67.1=pypi_0
"""
