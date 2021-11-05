# 该论文2005年由Sun、Yuan等人提出
论文：Image Completion with Structure Propagation



## 主要思想：十分详细解释：先要补全结构（线条）的小张图片，然后再补全纹理图片（就是非线条的地方）



# 缺点：必须先要自己动手画出缺失纹理的线条！！！

优点：线条小图片补全很全面，提出BP、DP和loop BP算法。都是有效补全线条小图片。

### 先计算自己画出线条的小图像其他图像的“距离”的小距离，再计算其他图像的匹配程度，最后再计算补全小图片重叠部分的匹配程度，三个加权求和构成的Loss，最小化loss，找到的小图片让Loss最小化即为应当用来补全的图片。

![image-20211105160534297](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20211105160534297.png)

