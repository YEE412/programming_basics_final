# programming_basics_final
final project of 《Programming Basics》RUC ISBD 2022 by Hu shiyu

## 数据集
数据集来源于 [燃气轮机CO和NOx排放数据](https://archive.ics.uci.edu/ml/datasets/Gas+Turbine+CO+and+NOx+Emission+Data+Set)。

预处理之后的数据集:"./data_preprocessed.csv"

## 项目简介
该数据集包含11个传感器在5年内测量的数值，用于研究燃气轮机的CO和NOx排放与环境参数及燃气轮机参数的关系。该数据集共有11列，由3个环境参数和6个燃气轮机参数以及CO和NOx排放量组成。本次项目的主要目的是希望能够利用环境参数和燃气轮机参数预测燃气轮机的CO和NOX的排放量，找到一个预测效果优良的预测模型。

## 主要思路
原数据集共有2011-2015五年的数据，因此选择前三年的数据作为训练集，后两年的数据作为验证集。本次项目拟合了两类共四个模型。由于该数据集的多重共线性程度很高，所以选择PCA和ridge regression来拟合模型，分别对响应变量是CO和NOX拟合两类共四个模型。另外还利用验证集计算了模型的预测误差，由此分析模型的优劣性。

## 复现说明
运行环境：system='Windows', release='10', version='10.0.19044', machine='AMD64'

numpy version: 1.22.4

pandas version: 1.4.2

seaborn version: 0.11.2

matplotlib version: 3.5.2

sklearn version: 1.1.1

sklearn version: 0.13.2

