# CSS总结1

## 引入css

### 行内式（权重高）

- style=“color：black；”

### 内联式

- 在head里面添加<style></style>

### 外链式

- <link rel="stylesheet" href="index.css">

## css样式

### 选择器 { 属性值： 值； 属性值： 值}

## css选择器

### 基础选择器

- id选择器
(id不能重复）

	- id="类名"
#类名 {   }

- 类选择器
（可以多次使用）

	- class=“类名  类名"
.类名 { }

- 标签选择器

	- h3 { color :red;}

- 通配符选择器
(会降低响应页面速度不推荐使用）

	- *{margin: 0;
padding:0;
}

## 字体

### 样式

- Unicode字体
（一般只用宋体和微软雅黑）

- font-style:  ;

	- 倾斜  italic
不倾斜  normal（工作中常用）

- font-weight :  ;

	- bold  加粗   ||  700不加单位
normal  不加粗  ||  400不加单位

- font-family :  ; 字体
- font-size: 25px;字号
- font 连写

	- 选择器{ font: font-style  font-weight  font-size/line-height  font-family;}
1.字体连写是有顺序的不能随意换位置2. 其中字号和字体必须同时出现

### 颜色
color

- 预定义的

	- 比如：red，black

- 十六进制

	- #FF0000

- RGB

	- rgb(255,0,0)
rgb(100%,0%,0%)

### text-align:  ;
文本水平对齐

- left
right
center

### line-height:  ;
行间距（一般比字号大7.8像素左右）

### text-indent: 2em ;
首行缩进

- 1em单位就是一个字的大小
（允许使用负值）

### text-decoration：  ;
文本线

- none  取消下划线
underline  下划线
overline  文本上一条线 （不用）
line-though  删除线（不常用）

## 盒子

### 边框
border：1px  solid  red
border-top/bottom/left/right

- 。none: 没有边框即忽略所有边框的宽度(默认值)
。solid: 边框为单实线(最为常用的)
。dashed: 边框为虚线
。dotted: 边框为点线

- border-collapse: collapse;
合并边框

### 内外边距
padding: 0 20px;
margin: 0 20px;

- 居中
margin：0 auto；

### 行内元素为了照顾兼容性，尽量只设置左右内外边距，不要设置上下内外边距。
width >padding>margin

- 解决塌陷添加
overflow：hidden;

### 圆角
border-radius: ;

### 阴影
box-shadow:水平阴影   垂直阴影   模糊距离(虚实)  阴影尺寸 (影子大小)    阴影颜色   内/外阴影;

## 复合选择器

### .nav  a {    }
后代选择器

### div>p{     }
子代选择器

### p.class{    }(中间不能有空格)
交集选择器（不常用）

### p,span,a{    }
并集选择器

### 伪类选择器

- a:link
未访问的链接
- a:visited
已访问的链接
- a:hover
鼠标移动到链接上
- a:active
选定的链接
- link>visited>hover>active

## 背景设置

### backgrond-color
backgrond-image:url()  括号不要加引号

### backgrond-repeat:   ;
平铺

- repeat(默认)背景在x，y上平铺
no-repeat
repeat-x
repeat-y

### 位置

- backgrond-position：x  y;

	- length   百分数/浮点数字和单位标识
position :top/center/bottom/left/right 

### 附着

- backgrond-attachment:  ;

	- scroll  随对象滚动
fixed  图像固定

### 简写

- backgrong: 背景颜色 背景图片地址  背景平铺  背景滚动  背景位置


### 背景透明

- background: rgba(0,0,0,0.3)
0.3为最后取值0~1之间为透明度

## 优先级取决于就近原则

### ！important级别最高

1) 如果选中了，那么以上面的公式来计权重。谁大听谁的。
2)如果没有选中，那么权重是0，因为继承的权重为0.
注：
权重相同执行就近原则

## 块级元素和行内元素

### 块级元素

- <h1>~<h6>
<p>    <div>
<ul>   <li>等

	- (1)比较霸道，自己独占-行
(2)高度，宽度、外边距以及内边距都可以控制。
(3)宽度默认是容器(父级宽度)的100%
(4)是一个容器及盒子，里面可以放行内或者块级元素。


### 行内元素

- (1)相邻行内元素在一行上，-行可以显示多个。
(2)高、宽直接设置是无效的。
(3)默认宽度就是它本身内容的宽度。
(4)行内元素只能容纳文本或则其他行内元素。
●链接里面不能再放链接。
●特殊情况a里面可以放块级元素，但是给a转换一下块级模式最安全。


### 行内块元素

- <img />
<input />
<td>

	- 可以设置高和宽
(1)和相邻行内元素(行内块)在-行上,但是之间会有空白缝隙。-行可以显示多个
(2)默认宽度就是它本身内容的宽度。
(3)高度，行高、外边距以及内边距都可以控制。


### 块级元素和行内元素相互转换

- display

	- inline
块转行
	- block
行转内
	- inine-block
块，行转为行内块

*XMind: ZEN - Trial Version*