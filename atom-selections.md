# Atom 文本选择

Atom 支持了很多文本选择操作，比如区域删除、缩进和一些查找操作，以及用引号或者括号把文字括起来之类的标记操作。

选择命令借鉴了很多移动命令命令。他们实际上与移动命令具有相同的快捷键，只不过加了个 `shift` 。

`ctrl-shift-P`：选择从当前位置到上一行的相同位置之间的内容

`ctrl-shift-N`：选择从当前位置到下一行的相同位置之间的内容

`ctrl-shift-B`：选择前一个字符

`ctrl-shift-F`：选择后一个字符

`alt-shift-B`, `alt-shift-left`：选择从当前位置到单词开头之间的内容

`alt-shift-F`, `alt-shift-right`：选择从当前位置到单词末尾之间的内容

`ctrl-shift-E`, `cmd-shift-right`：选择从当前位置到本行末尾之间的内容

`ctrl-shift-A`, `cmd-shift-left`：选择从当前位置到本行开头之间的内容

`cmd-shift-up`：选择从当前位置到文件开头之间的内容

`cmd-shift-down`：选择从当前位置到文件底部之间的内容


除了通过移动光标来进行选择之外，还有一些方便选择内容的特定区域的命令。


`cmd-A`：选择整个缓冲区

`cmd-L`：选择整行

`ctrl-shift-W`：选择当前单词
