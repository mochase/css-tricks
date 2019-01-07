@keyframes
animation

animation-delay
延迟

animation-direction: <normal> | <alternate> | <reverse> | <alternate-reverse>
运行方向
normal: 0 -> 1 --- 0 -> 1
reverse: 1 -> 0 --- 1 -> 0
alternate: 0 -> 1 -> 0 -> 1
alternate-reverse: 1 -> 0 -> 1 -> 0

animation-duration
一个周期的时长

animation-fill-mode: <none> | <forwards> | <backwards> | <both>
动画首尾的样式填充
none: A --- A(delay, 如果有) --- 0 -> 1 --- A
forwards: A --- 0 -> 1 --- 1
backwards: A --- 0(delay, 如果有) --- 0 -> 1 --- A
both: forwards + backwards


animation-iteration-count
循环次数,可以为小数

animation-name

animation-play-state: <running> | <paused>
提供暂停的功能

animation-timing-function