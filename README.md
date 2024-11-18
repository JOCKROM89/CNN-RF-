# CNN-RF
Use CNN-RF to  Identify images

使用卷积神经网络和随机森林来实现对图像集的辨别分类
## 环境
* Python 3.10及以上
* Pytorch
* CIFAR 10图像集
## 数据集

CIFAR-10 数据集由 10 个类的 60000 张 32x32 彩色图像组成，每个类有 6000 张图像。有 50000 张训练图像和 10000 张测试图像。

数据集分为 5 个训练批次和 1 个测试批次，每个批次有 10000 张图像。测试批次包含每个类中随机选择的 1000 张图像。训练批次包含按随机顺序排列的剩余图像，但某些训练批次可能包含来自一个类的图像多于另一个类的图像。在它们之间，训练批次包含来自每个类的 5000 张图像。
以下是数据集中的类，以及每个类的 10 张随机图像：

![image](https://github.com/JOCKROM89/CNN-RF/blob/master/data/Snipaste_2024-11-18_09-18-54.png)

下载地址：https://www.cs.toronto.edu/~kriz/cifar.html

## CNN模型
具体代码参考cnn_model.py
该模型是由4个卷积层、2个池化层、2个全连接层构成
