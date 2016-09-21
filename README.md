
## 为了达到上面效果图的手势动画效果，我们必须做如下设置，通过app:layout_scrollFlags=”scroll|enterAlways”属性来确定哪个组件是可滑动的

###设置的layout_scrollFlags有如下几种选项：

    1.scroll:               所有想滚动出屏幕的view都需要设置这个flag- 没有设置这个flag的view将被固定在屏幕顶部。

    2.enterAlways:          这个flag让任意向下的滚动都会导致该view变为可见，启用快速“返回模式”。
   
    3.enterAlwaysCollapsed: 当你的视图已经设置minHeight属性又使用此标志时，你的视图只能已最小高度进入，只有当滚动视图到达顶部时才扩大到完整高度。

    4.exitUntilCollapsed:   滚动退出屏幕，最后折叠在顶端。

## RecyclerView实现了拖拽排序效果

## 这里使用的gradle版本为：classpath 'com.android.tools.build:gradle:2.0.0'

## 效果图：
![](http://i.imgur.com/ZSDUri2.gif)

