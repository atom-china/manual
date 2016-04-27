# Atom Flight Manual

翻译自 <http://flight-manual.atom.io>

## 已翻译内容索引

* [第一章：新手入门](./chapter-1-getting-started/)
    * [为什么选择 Atom？](./chapter-1-getting-started/why-atom.md)
    * [Atom 基础](./chapter-1-getting-started/atom-basics.md)
    * [安装 Atom](./chapter-1-getting-started/installing-atom.md)
* [第二章：使用 Atom](./chapter-2-using-atom/)
    * [Atom 文本选择](./chapter-2-using-atom/atom-selections.md)

## 如何参与翻译

1. 在 [翻译认领](https://github.com/atom-china/manual/issues?q=is%3Aissue+is%3Aopen+label%3A翻译认领) 列表中认领翻译章节，在 Issue 下添加评论认领。
2. 为了避免重复工作，请在仓库维护者确认之后，Fork 此仓库开始翻译，翻译请遵循 [排版约定](#排版约定)。
3. 翻译完成后，发送 Pull Request，并在原 Issue 添加链接。
4. 处理校对者的校对建议。

> 建议：Fork 此仓库后，请先从 master 分支上 `git checkout -b translate` 一个新的 translate 分支来翻译文章，翻译完成后再把 translate 分支发 PR。

## 如何参与校对

1. 在 [校对认领](https://github.com/atom-china/manual/issues?q=is%3Aissue+is%3Aopen+label%3A校对认领) 列表中认领校对章节。
2. 直接在翻译章节对应的 Pull Request 里添加 note 校对，校对时可参考 [排版约定](#排版约定)。

> 在文章被认领之后也欢迎小伙伴继续添加 note，共同目的都是提高翻译质量。

## 其它参与方式

如果你在阅读过程中发现翻译错误，或与 master 分支内容与官方手册不同步，你可以发一个 Issue 提醒该仓库的维护者关注这个问题，或者你也可以直接发起 Pull Request 来修正这个错误。

## 排版约定

* 中英文之间需要使用空格。

  例如：

  ```
  这个仓库托管在 GitHub 上。
  ```

* 嵌套在内容里的超链接前后使用空格。

  例如：

  ```
  可以从 <https://atom.io> 获取 Windows Installer
  ```

* code 标记原则上尽量忠实原文，但额外给所有包含符号的命令、路径都添加 code 标记。

  例如：

  ```
  当 Atom 启动后它会在 `%USERPROFILE%` 下创建 `.atom` 文件夹
  ```

## 参考链接

在 GitHub 上有一些前人针对这个手册进行了一些翻译工作，翻译者可以参考：

* <https://github.com/wizardforcel/atom-flight-manual-zh-cn>
* <https://github.com/guo-yu/atom-guide>

感谢他们和所有参与者的工作！
