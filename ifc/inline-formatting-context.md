原文地址: https://www.w3cplus.com/css/css-font-metrics-line-height-and-vertical-align.html

##关于inline-formatting-context, vertical-align, line-height, inline盒子模型##
一点笔记:
+ 字体度量单位em(em-square), ex(小写字母x), px的含义.
+ content-area(因字体的度量而异. font-size * 系数n).
+ virtual-area(由line-height定义)
+ line-height的真正含义(css中不是baseline之间的距离).初始值normal是相对于font-size而言.不同字体的默认line-height不同(也因浏览器而异).
+ content-area始终垂直方向上居中于virtual-area.
+ 手动设置line-height为1很愚蠢.(导致virtual-area < content-area)
+ line-box的高度的计算方式
+ line-box的`strut`对于baseline确定的意义.(自身的字体,line-height)
+ vertical-align: top, bottom / baseline, text-top, text-bottom的区别
+ `vertical-align: bottom` ---- 自身的virtual-area底端与整个line-box底端对齐
+ `vertical-align: text-bottom` ---- 父元素strut的content-area底端与自身的virtual-area底端对齐.
+ `vertical-align: middle` ---- Middle “aligns the vertical midpoint of the box with the baseline of the parent box plus half the x-height of the parent”.
