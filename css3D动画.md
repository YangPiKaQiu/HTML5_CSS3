# css3D动画

### z的数值正数是向我们眼前移动

## perspective
透视

## 3D呈现
transfrom-style

### ●控制子元素是否开启三维立体环境。。
●transform-style: flat子元素不开启3d立体空间默认的
●transform-style: preserve- 3d;子元素开启立体空间.
●代码写给父级,但是影响的是子耔
●这个属性很重要,后面必用


## 旋转
rotate3d

### 左手准则   X轴（大拇指朝右）
●左手的手拇指指向x轴的正方向
●其余手指的弯曲方向就是该元素沿着x轴旋转的方向


### ●transform:rotateX(45deg) :沿着x轴正方向旋转45度
●transform:rotateY(45deg) : 沿着y轴正方向旋转45deg
●transform:rotateZ(45deg) : 沿着Z轴正方向旋转45deg
●transform:rotate3d(x,y,z,deg) :沿着自定义轴旋转deg为角度(了解即可)


### ●,左手的手拇指指向y轴的正方向（大拇指朝下）
●其余手指的弯曲方向就是该元素沿着y轴旋转的方向(正值)


### transform:rotate3d(xy,z,deg) :沿着自定义轴旋转deg为角度(了解即可)
xyz是表示旋转轴的矢量,是标示你是否希望沿着该轴旋转，最后一个标示旋转的角度。


## 私有前缀

*XMind: ZEN - Trial Version*