**2020.2.7**  
**Author : [YHUAN](https://github.com/yhuan416)**  
**这个点阵操作库是我自己写的,用于SSD1306 OLED 模块的操作**  

# 目录简介

*Easy_Bitmap文件夹是库文件的本体*

*Easy_Font是支持的字体格式*

---

# 使用说明

1. 配置显示缓冲区的大小 (bit)  
> #define GRAM_W	(128)  
> #define GRAM_H	(64)  

2. 显示一个像素点  
```
	void bitmap_DrawPixel(unsigned char *gram, unsigned int x, unsigned int y, unsigned char mask);
```
> gram : 需要操作的缓冲区  
> (x, y) : 像素的位置  
> mask : 置一或清零  

3. 显示一个字符  
```
	void bitmap_DrawChar(unsigned char *gram, int x, int y, char ch, _FontDef *font);
```
> gram : 需要操作的缓冲区  
> (x, y) : 字符显示的位置  
> ch : 要显示的字符  
> font : 使用的字体  


---

