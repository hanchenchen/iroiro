# DCT for Discrete Cosine Transform

DCT 是无损的，它只将图像从空间域转换到变换域上，使之更能有效地被编码。

```matlab
clear                             %清除工作区间
RGB=imread('G:\MATLAB\bm.bmp');   %加载图片
GRAY=rgb2gray(RGB);               %彩色转灰度图
figure,imshow(GRAY);               %显示灰度图
D=dct2(GRAY);                     %进行dct变换
figure,imshow(log(abs(D)),[ ]);   %显示变换过程
colormap(gray(4));colorbar;
D(abs(D)<0.1)=0;
I=idct2(D)/255;                   %设置限值
figure,imshow(I)                %显示变换后的图
```







##### Reference

[DCT变换][https://blog.csdn.net/timebomb/article/details/5960624]

[MATLAB中的DCT实现][https://blog.csdn.net/dyq1995/article/details/86149368]

