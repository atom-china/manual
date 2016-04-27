# 在 Atom 里移动

虽然使用鼠标和方向键在 Atom 里移动已经足够简单，Atom 还额外提供了一些快捷键，能让你的手不用离开键盘，更快地在文档中导航。

首先，Atom 自带了许多 Emacs 快捷键用于在文档中导航。你可以使用 `ctrl-P` 和 `ctrl-N` 来将光标上移或下移一个字符，使用 `ctrl-B` 和 `ctrl-F` 将光标左移或右移一个字符。这和使用方向键是一样的，但有些人不喜欢把手移到方向键的位置。

除了以单个字符为单位的移动，还有许多其它用于移动的快捷键。

`alt-B`，`alt-left`：移到词首

`alt-F`，`alt-right`：移到词尾

`cmd-right`，`ctrl-E`：移到行尾

`cmd-left`，`ctrl-A`：移到本行第一个字符

`cmd-up`：移到文件开头

`cmd-down`：移到文件末尾

你也可以使用 `ctrl-G` 直接移动到某一行（和列），按 `ctrl-G` 后会弹出一个对话框询问你想跳到哪一行，也可以输入 `row:column` 来跳到那一行的某个字符。

![Go directly to a line](./images/goto.png)

图 1. 直接跳到某一行

## 通过符号（Symbols）导航
