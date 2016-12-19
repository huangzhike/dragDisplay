# dragDisplay
拖动展示，模仿[豪情的作品](http://jikeytang.github.io/slide/05/index.html)

原理是分两层，底层图片（黑色部分）和绝对定位的上层。上层容器内的图片（白色部分）也需要固定位置，通过监听鼠标的位移来改变上层容器的宽度，形成拖动效果。

**与豪情的主要区别：**

* 拖动的图标相对父容器绝对定位，不需要通过JS改变，豪情作品是通过JS同时改变了父容器宽度与图标的位置；
* 代码更简单；
* 位移的计算更简单，豪情作品是计算了鼠标与图标的距离，引入了许多中间变量，我直接通过鼠标位移改变宽度，更加方便，同时流畅度提升，鼠标拖动更“黏手”。
* 添加了移动端的支持；
* 其它可以参见代码。
