# css2D动画

## 2D动画

### transform

- ●定义2D转换中的移动,沿着X和Y轴移动元素
●translate最大的优点:不会影响到其他元素的位置
●translate中的百分比单位是相对于自身元素的translate:(50%, 50%);
●对行内标签没有效果

- translate
2D转换之移动

	- transformn: translate(x,y);
或者分开写
transforem: translateX (n) ;
transform: translateY (n) ;


- rotate
旋转

	- transform：rotate（度数）

		- ●rotate里面跟度数，单位是deg比如rotate(45deg)
●角度为正时,顺时针,负时,为逆时针
●默认旋转的中心点元素的中心点

- transform-origin
旋转中心点

	- transform-origin：x y； 

		- ●注意后面的参数x和y用空格隔开
●xy默认转换的中心点是元素的中心点(50% 50%)
还可以给xy设置像素或者方位名词( top bottom left right center )


- scale
缩放

	- transform:scale(x,y);

		- 注意其中的x和y用逗号分隔
●transform:scale(1,1) : 宽和高都放大-倍,相对于没有放大
●transform:scale(2,2) : 宽和高都放大了2倍
●transform:scale(2) : 只写一个参数, 第二个参数则和第一个参数- 样,相当于scale(2,2)
●transform:scale(0.5,0.5) :缩小
sacle缩放最大的优势:可以设置转换中心点缩放,默认以中心点缩放的,而且不影响其他盒子


- 综合写法

## 过渡
transition

### 过渡写到本身上，谁做动画给谁加
transition：all  0.3s；

## 动画
animation

- 动画序列
●0% 是动画的开始, 100%是动画的完成。这样的规则就是动画序列。
●在@keyframes中规定某项CSS样式,就能创建由当前样式逐渐改为新样式的动画效果。
●动画是使元素从一种样式逐渐变化为另-种样式的效果。 您可以改变任意多的样式任意 的次数。
●请用百分比来规定变化发生的时间 ,或用关键词"from"和"to" ,等同于0%和100%。

### 动画属性

### animation :动画名称   持续时间   运动曲线   何时开始   播放次数   是否反方向   动画起始或者结束的状态;


*XMind: ZEN - Trial Version*