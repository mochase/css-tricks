`flex`: 下面三个属性的缩写
`flex-grow`
`flex-shrink`
`flex-basis`

`flex-flow`: 下面两个属性的缩写
`flex-direction`: flex 的方向
`flex-wrap`: item 是否换行

`align-items`: 行内的 item 垂直轴方向排列
`align-self`单个 item 的垂直轴方向排列
`align-content`: 行与行之间的垂直轴方向排列(多行才生效)

`justify-content`: 行内的 item 水平轴方向的排列

`order`

## flex 的一些缩写含义

auto => 1 1 auto
initial => 0 1 auto
none => 0 0 auto
number => number 1 0

## min-width / min-height
默认情况下 item 最小收缩到它的 content-size, 使用 min-width 可以改变这个临界值

## flex 宽度计算规则
基于 flex-basis, grow 时不加权, shrink 时加权
grow 情况下: `item with = basis +  delta width *  grow  / (∑i grow )`
shrink 情况下: `item width = basis - delta width * (shrink * basis ) / (∑i shrink * basis))`

## 计算 basis 的优先级
flex-basis > width > content-size

