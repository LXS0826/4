# RBFN Classification for Multiple Datasets

这个项目使用径向基函数网络 (RBFN) 对多个数据集进行分类，包括 MNIST 手写数字数据集、肺部疾病数据集和 Yale 人脸数据集。该模型利用高斯核作为基函数，并在 PyTorch 框架下实现。

## 安装指南

在开始之前，确保你已经安装了 Python 和以下必要的库：

- numpy
- scipy
- torch

你可以使用 `pip` 命令来安装缺失的库：

```bash
pip install numpy scipy torch
数据集
数据集应该以 .mat 格式存储，并放置在 datasets 文件夹中。确保你有以下数据集的路径：

MNIST 数据集: datasets\MNIST.mat
肺部疾病数据集: datasets\lung.mat
Yale 人脸数据集: datasets\Yale.mat
使用方法
克隆这个仓库到你的本地机器上：
git clone https://github.com/your-username/rbfn-classification.git
cd rbfn-classification
运行主脚本：
python rbfn_script.py
RBFN 模型
RBFN 类是一个 PyTorch 模块，使用高斯核作为径向基函数。模型初始化时需要指定中心点和输出类别的数量。

训练与测试
脚本将自动执行以下步骤：

加载数据集并拆分为训练集和测试集。
初始化 RBFN 模型。
对每个数据集进行多次迭代训练，并在测试集上评估模型性能。
打印每个数据集的最高准确率。
