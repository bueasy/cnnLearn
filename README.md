# cnnLearn

CNN主要在应用在图像识别领域。CNN对图像的处理跟脑对外界图像的处理原理上一致：
## 获取外界图像
当人眼观察一个事物的时候，并不是每个视神经细胞感知所有看到的“像素”，而是一个神经细胞负责一小块视野，也就是说假设看到的全部视野是1000像素，而神经细胞有10个，那么一个神经细胞就负责比1000/10得到的平均值大一圈的范围，也就是200像素，一个细胞负责200个像素，10个细胞一共是2000个像素，大于1000个像素，说明有重叠。
## 特征提取
如果把外界图像表示为5*5的矩阵，每个神经细胞能感受到的图像的矩阵是3*3，那么，卷积核的大小就是3*3，感受野的大小也是3*3。
特征提取的过程就是拿着卷积核以此扫描源图像矩阵，因此卷积核也称之为过滤器/滤波器/滤波矩阵，卷积应用也称之为滤波。
特征提取就是源图像和滤波矩阵进行逐个元素相乘再求和的操作。
## 特征学习
自动化地获取卷积核对应矩阵的值的过程称之为特征学习。

## 池化层
对输入的特征图进行压缩，一方面使特征图变小，简化网络计算复杂度；一方面进行特征压缩，提取主要特征。
池化操作一般有两种，一种是Avy Pooling,一种是max Pooling，也就是说池化就是把很多数据用最大值或者平均值代替，目的是降低数据量。

## 卷积定理和快速傅里叶变换
卷积定理：时域上的卷积等于频域上的乘积
http://www.qiujiawei.com/convolution/
https://zhuanlan.zhihu.com/wille/19763358
https://zhuanlan.zhihu.com/p/23739221

