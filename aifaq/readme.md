# 机器学习
## 机器学习的分类
## 梯度下降在机器学习中的应用
# 神经网络
## 神经网络与机器学习的关系
## Back Propagation算法
## Back Propagation算法的缺点
不会去调整无关参数
## 为什么神经网络有效
## 监督学习
## 网络学习的问题
## Softmax
## CNN
### 为什么CNN有效
  * [谷歌NN教程](https://classroom.udacity.com/courses/ud730)里讲得是CNN将平面数据逐步转换成金字塔型数据
  * 需要识别的部分只占用图片的很小一部分
  * 缩小图片，同样能够识别图片
  * 平移目标，同样识别图片
  * 通过共享Weight实现了一个小的filter
  * 通过MaxPool实现了缩小图片
  * 输入只与Filter相关Netron连接，大幅减少了运算量
