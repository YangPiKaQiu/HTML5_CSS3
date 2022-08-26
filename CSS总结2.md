# CSS总结2

## 浮动

### float：left/right

### 使用后相当于转换成行内块元素

### 清除浮动

- clear：right/left/both(清除两侧浮动)

	- 在浮动的元素最后面加上空标签
写上clear：both；
	- 自由主题

## 定位

### 静态定位

- staic

	- 没有边偏移

### 绝对定位

- absolute

	- 1.完全脱标- -一 完全不占位置;
2.父元素没有定位，则以浏览器为准定位(Document 文档)。

		- top
right
bottom
left
		- 想要居中就设置属性50%
		- 1.[ left: 50%; ]: 让盒子的左侧移动到父级元素的水平中心位置;
2.margin-left: -100px;]: 让盒子向左移动**自身宽度的-半** 。

### 固定定位

- fixed

	- 贴近内容，只需要版心的一半50%加上自己本身的宽度

### 相对定位

- relative

	- 相对定位是元素相对于它原来在标准流中的位置来说的。(自恋型)
相对于自己原来在标准流中位置来移动的
原来**在标准流的区域继续占有**,后面的盒子仍然以标准流的方式对待它。

### z-index: 正负整数不要小数
数值越大越在上面

- 不用加单位
| z- index只能应用于相对定位、绝对定位和固定定位的元素， 其他标准流、浮动和静态定位无效。


### 行内块属性绝对|相对|浮动都可以转成行内块元素

### display：none;
隐藏元素不在占有位置

- block
显示元素并转换成块级元素

## visibility：
显示或隐藏

### hidden：隐藏元素保留位置
visible：显示元素保留位置

## overflow：
溢出

### visible 不剪切内容也不加滚动条
hidden超出部分影藏不显示
scroll 不管是否超出都加上滚动动条
auto 超出显示滚动条，不超出不显示

## cursor:
鼠标样式

### default 小白  默认
pointer  小手
move 移动
text 文本
not-allowed 禁止

## 文本框去除
outline：

### none

## 结构伪类选择器

### E:first-child
父元素中的第一个子元素

### E: last-chaild 
父元素中最后一个子元素

### E: nth-child(n)
匹配父元素中第n个子元素

- even 偶数
odd  奇数

### E: first-of-type
指定类型E的第一个

### E:last-of-type
指定类型最后一个

### E:nth-of-type(n)
指定类型E的第n个

## 伪元素选择器

### ：：before
在元素内部前面插入内容

### ：：after
在元素内部后面插入内容

*XMind: ZEN - Trial Version*