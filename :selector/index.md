# 部分伪类选择器比较与归类(:link, :visited, :hover, :active, :focus)

`:link` 与 `:visited`特指 a 标签的两种状态: 未被访问与已被访问
`:hover` 与 `:active` 适用所有元素. `hover` -- 鼠标悬停, `active` -- 鼠标按住不放

超链接的4种状态，需要有特定的书写顺序才能生效。 正确顺序 link -> visited -> hover -> active (记忆: love hate)

`focus`: 特指输入框(input 等), 触发 focus 事件时被选中