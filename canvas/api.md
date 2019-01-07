# 一些 api

## 基本操作

beginPath()
closePath()
stroke()
fill()
moveTo()

## 线条操作

lineTo(x, y)
rect(x,y,width,height)
绘制矩形(绘制开始前自动moveTo(x,y))
arc(x, y, r, startArc, endArc, direction)
绘制圆弧
quadraticCurveTo(cpx, cpy, x, y)
绘制二次贝塞尔曲线，cp1x,cp1y为一个控制点，x,y为结束点。
bezierCurveTo(cp1x,cp1y,cp2x,cp2y, x, y)
绘制三次贝塞尔曲线，cp1x,cp1y为控制点一，cp2x,cp2y为控制点二，x,y为结束点。

## Path2D 对象

用来封装一系列 path 操作,简化代码,同时可以导入 svg 格式 path
```
var p = new Path2D('M10 10 h 80 v 80 h -80 Z');
```

## 色彩

fillStyle
strokeStyle
globalAlpha

## Line styles

lineWidth
lineCap(butt | round | square)
lineJoin
miterLimit
getLineDash
setLineDash
lineDashOffset

## 渐变

lineargradient
radialgradient

## Patterns

createPattern

## 绘制文本

fillText
strokeText

## 绘制图像

drawImage

1. 简单绘制 （image, x, y）

2. 缩放图像 （image, x, y, width, height）

3. 切片 (image, x, y, width, height, dx, dy, dwidth, dheight)

前4个是定义图像源的切片位置和大小，后4个则是定义切片的目标显示位置和大小。

## 状态的保存与回退

save()
restore()

## 变形

translate(x, y)
rotate(angle)
scale(x, y)
transform(m11, m12, m21, m22, dx, dy)

## 合成与裁剪

globalCompositeOperation = type
clip()

## 像素操作

ImageData 对象
createImageData()
getImageData(left, top, width, height)
putImageData(imageData, dx, dy)
toDataURL()