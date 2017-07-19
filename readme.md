[TOC]

## 1. 二维码简介

### 1.1 定义
- 2-dimensional bar code
- 用某种特定的几何图形按一定规律在平面（二维方向上）分布的黑白相间的图形记录数据符号信息

### 1.2 分类
- 码制：Data Matrix, Maxi Code, Aztec, QR Code, Vericode, PDF417, Ultracode, Code 49, Code 16K等
- 堆叠式/行排式二维条码
    - 又称堆积式二维条码或层排式二维条码
    - 编码原理是建立在一维条码基础之上，按需要堆积成二行或多行
    - Code 16K、Code 49、PDF417、MicroPDF417 等
- 矩阵式二维码
    - 又称棋盘式二维条码
    - 在一个矩形空间通过黑、白像素在矩阵中的不同分布进行编码
    - 用点（方点、圆点或其他形状）的出现表示二进制“1”，点的不出现表示二进制的“0”
    - Code One、MaxiCode、**QR Code**、 Data Matrix、Han Xin Code、Grid Matrix
    - Quick Response Code

### 1.3 特点
- 存储量大
    - 传统的条形码只能处理20位左右的信息量，QR码可处理条形码的几十倍到几百倍的信息量
    - 所有数据类型 - 数字、英文字母、日文字母、汉字、符号、二进制、控制码等

![img](file:///var/folders/29/srh45zys4lz9whn2qdkcwxdc0000gn/T/WizNote/75cefb8a-fcbe-4543-a6e0-13e4037478d8/index_files/73201728.png)

- 空间小
    - QR码使用纵向和横向两个方向处理数据，如果是相同的信息量，QR码所占空间为条形码的十分之一左右
    - Micro QR码，更小

![img](file:///var/folders/29/srh45zys4lz9whn2qdkcwxdc0000gn/T/WizNote/75cefb8a-fcbe-4543-a6e0-13e4037478d8/index_files/72706027.png)

- 支持各种字符
  - 日本人发明，非常适合处理日文和汉字
- 对变脏和破损的适应能力强
  - 纠错功能，即使部分编码变脏或破损，也可以恢复数据
  - 最多可纠错约30%
- 从任意方向读取

![img](file:///var/folders/29/srh45zys4lz9whn2qdkcwxdc0000gn/T/WizNote/75cefb8a-fcbe-4543-a6e0-13e4037478d8/index_files/73083322.png)

- 支持合并
  - QR码可以将数据分割为多个编码，最多支持16个QR码

![img](file:///var/folders/29/srh45zys4lz9whn2qdkcwxdc0000gn/T/WizNote/75cefb8a-fcbe-4543-a6e0-13e4037478d8/index_files/73088194.png)

### 1.4 QR码

#### 1.4.1 版本

> 码元：构成QR码的方形黑白点

- 设有1-40的不同版本（种类）
- 每个版本都具备固有的码元
- 版本1: 21x21
- 横纵向各以4码元为单位递增
- 版本40: 177x177

![img](file:///var/folders/29/srh45zys4lz9whn2qdkcwxdc0000gn/T/WizNote/75cefb8a-fcbe-4543-a6e0-13e4037478d8/index_files/74111425.png)

#### 1.4.2 纠错级别

- [里德-所罗门码](https://zh.wikipedia.org/wiki/%E9%87%8C%E5%BE%B7-%E6%89%80%E7%BD%97%E9%97%A8%E7%A0%81)  [Reed-Solomon码的解释](https://www.felix021.com/blog/read.php?2116) [S编码和纠错算法](http://read.pudn.com/downloads210/ebook/986946/RS/RS%E7%BC%96%E7%A0%81%E5%92%8C%E7%BA%A0%E9%94%99%E7%AE%97%E6%B3%95.pdf)


- 4个级别，根据环境选择
- 级别提高 -> 纠错能力提高 -> 数据量增加 -> 编码尺寸增加

![img](file:///var/folders/29/srh45zys4lz9whn2qdkcwxdc0000gn/T/WizNote/75cefb8a-fcbe-4543-a6e0-13e4037478d8/index_files/74954455.png)

#### 1.4.1 结构

![img](file:///var/folders/29/srh45zys4lz9whn2qdkcwxdc0000gn/T/WizNote/75cefb8a-fcbe-4543-a6e0-13e4037478d8/index_files/74244402.png)

![img](file:///var/folders/29/srh45zys4lz9whn2qdkcwxdc0000gn/T/WizNote/75cefb8a-fcbe-4543-a6e0-13e4037478d8/index_files/74253509.png)