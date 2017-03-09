
### 为了达到上面效果图的手势动画效果，我们必须做如下设置，通过app:layout_scrollFlags=”scroll|enterAlways”属性来确定哪个组件是可滑动的

#### 设置的layout_scrollFlags有如下几种选项：

    1.scroll:               所有想滚动出屏幕的view都需要设置这个flag- 没有设置这个flag的view将被固定在屏幕顶部。

    2.enterAlways:          这个flag让任意向下的滚动都会导致该view变为可见，启用快速“返回模式”。
   
    3.enterAlwaysCollapsed: 当你的视图已经设置minHeight属性又使用此标志时，你的视图只能已最小高度进入，只有当滚动视图到达顶部时才扩大到完整高度。

    4.exitUntilCollapsed:   滚动退出屏幕，最后折叠在顶端。
    
### CollapsingToolbarLayout的一些属性

#### app:contentScrim="#1dcdef" 设置当完全CollapsingToolbarLayout折叠(收缩)后的背景颜色

#### app:expandedTitleMarginStart="48dp"//设置扩张时候(还没有收缩时)title向左填充的距离

#### app:layout_collapseMode="parallax"//设置为这个模式时，在内容滚动时，CollapsingToolbarLayout中的View（比如ImageView)也可以同时滚     动，实现视差滚动效果，通常和layout_collapseParallaxMultiplier(设置视差因子)搭配使用

#### app:layout_collapseParallaxMultiplier="0.7"//设置视差滚动因子，值为：0~1

#### app:layout_collapseMode="pin"//pin设置为这个模式时，当CollapsingToolbarLayout完全收缩后，Toolbar还可以保留在屏幕上

#### RecyclerView实现了拖拽排序效果

### 效果图：
![](http://img.blog.csdn.net/20161020100053315)

#### CSDN博客地址：[http://blog.csdn.net/a_zhon/article/details/52611166](http://blog.csdn.net/a_zhon/article/details/52611166)
#### 如果你遇到了什么问题，可以与我联系。
# LICENSE
The MIT License (MIT)

Copyright (c) 2015 阿钟
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

