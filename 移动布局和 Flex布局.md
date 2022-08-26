# 移动布局和
Flex布局

## 视口
viewport

### 布局视口
layout viewport

### 视觉视口(用户正在看到的网站的区域。注意:是网站的区域。)
visual viewport

### 理想视口
ideal viewport

●为 了使网站在移动端有最理想的浏览和阅读宽度而设定
●理想视口， 对设备来讲,是最理想的视口尺时
●需要手动添写meta视口标签通知浏览器操作
●meta视口标签的主要目的 :布局视C的宽度应该与理想视口的宽度-致,简单理解就是设备有多宽,我们布局的视口就多宽


## ●flex- direction :设置主轴的方向
●justify-content :设置主轴上的子元素排列方式
●
flex-wrap :设置子元素是否换行
●align-content :设置侧轴上的子元素的排列方式(多行)
●align-items :设置侧轴上的子元素排列方式(单行)
●flex-flow :复合属性,相当于同时设置了flex-direction和flex-wrap


## 多倍图

## 特殊样式

### /+css3盒子模型*/ 
box- sizing: border -box ;
-webkit -box - sizing: border -box;
/*点击高亮我们需要清除清除设 置为transparent完成透明/
-webkit-tap-highlight-color: transparent;
/*在移动端浏览器默认的外观在ios.上加上这个属性才能给按钮和输入框自定义样式*/
-webkit- - appearance: none ;
/*禁用长按页面时的弹出菜单*/
img,a { -webkit- touch- callout: none; }


## 二倍图

### 3.3背景缩放background-size
background-size属性规定背景图像的尺寸
background-size:背景图片宽度背景图片高度;
●单位:
长度I百分比Icover Icontain;
●cover把背景图像扩展至足够大,以使背景图像完全覆盖背景区域。
●contain把图像图像扩展至最大尺寸,以使其宽度和高度完全适应内容区域


## box-sizing:border-box;
不会因为内边距而撑大盒子

## meta
视口标签

## flex-wrap
设置子元素是否换行

### nowrap
默认值，不换行

### warp
换行

## flex-flow
是flex-direction和flex-wrap属性的复合属性

### flex-flow：row wrap；

## order定义项目排列顺序

### 数值越小，排列越靠前，默认为0
注意：和z-index不一样

## align-self（写在儿子元素里面，其他写在父级元素）
控制子项在侧轴排列

### align-self属性允许单个项目有与其他项目不一样的对齐方式 ,可覆盖align-items属性。
默认值为auto ,表示继承父元素的align-items属性,如果没有父元素,则等同于stretch。
span:nth-child(2) {
/*设置自己在侧轴上的排列方式*/
align-self: flex-end;
}


## align-items（单行）
设置主轴上子元素排列

### flex-start
从上到下

### flex-end
从下到上

### center
垂直居中

### stretch
拉伸

## flex-shrink
默认拉伸值为1
对宽度起效果

### 关闭拉伸值为0

## align-content（多行）
设置侧轴上子元素

### flex-start
设置侧轴头部元素

### flex-end
在侧轴尾部开始排列

### center
在侧轴中间显示

### space-around
子项在侧轴平分剩余空间

### space-between
子项在侧轴平分两天，在平分剩余空间

### stretch
设置子项元素平分父元素高度

## flex属性
定义子项目分配剩余空间，用flex占多少份数

### .item{
    flex：2；/*默认为零*/
}

## justify-content
设置主轴上的子元素排列

### flex-start
默认值从头开始 如果主轴是X轴，则从左到右

### flex-end
从尾开始排列

### center
在主轴居中对齐

### space-around
平分剩余空间

### space-between
先平分贴边 在平分剩余空间（*）

## 设置flex布局

### display：flex；

## align-content 和align-items区别

### ●align-items适用于单行情况下，只有上对挤、下对挤、居中和拉伸
●align-content适应于换行(多行)的情况下(单行情况下无效)，可以设置上对齐、下对齐、 居中、拉伸以及平均分
配剩余空间等属性值。
●总结就是 单行找align-items多行找align-content


## flex-direction
设置主轴方向

### row
默认从左到右

### row-reverse
从右到左

### column
从上到下

### column-reverse
从下到上

*XMind: ZEN - Trial Version*