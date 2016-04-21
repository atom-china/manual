## 安装 Atom

想要使用 Atom，我们就得先安装它。这部分将会讲到如何在 Mac，Windows 和 Linux 上安装 Atom，以及如何从源码构建它。

在上述系统下安装 Atom 都很简单。访问 <https://atom.io> 后在页面顶部你就能看到下载按钮。

![Download buttons on atom io](./images/linux-downloads.png)

图 1. atom.io 网站的下载按钮

这些按钮的文字和行为会自动对应你的操作系统，下载和安装都很方便。但我们还是一起详细看看吧！

### 给 Mac 安装 Atom

Atom 最初就是为 Mac 环境构建的，所以安装过程非常简单。可以直接点击 atom.io 网站上的下载按钮，也可以访问 Atom 的发布页：

<https://github.com/atom/atom/releases/latest>

在这个页面直接下载 `atom-mac.zip` 文件。

待文件下载完成后，点击解压，然后拖拽解压出来的 `Atom` 程序到你的 「Applications」 文件夹。

当你第一次打开 Atom 时，它会尝试安装终端下使用的 `atom` 和 `apm` 命令。在某些情况下，可能会因为需要管理员密码而安装失败。要检查 `atom` 命令是否安装成功可以打开一个终端然后运行 `which atom`，如果 `atom` 命令安装好了，会看到这样的输出：

```sh
$ which atom
/usr/local/bin/atom
$
```

如果 `atom` 命令没有安装，`which` 命令不会有输出：

```sh
$ which atom
$
```

想要自己安装 `atom` 和 `apm` 命令，可以在 Command Palette 运行 「Windows: Install Shell Commands」，会自动弹框询问你的管理员密码。（译注：Windows 下打开 Command Palette 的快捷键是 <kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>p</kbd> 。）

### 给 Windows 安装 Atom

在 Windows 下获取 Atom 可以从 <https://atom.io> 获取 Windows Installer，也可以从 [Atom Releases](https://github.com/atom/atom/releases/latest) 下载 AtomSetup.exe。

它们会帮你安装好 Atom，将 `atom` 和 `apm` 命令添加到 `PATH` 环境变量，在桌面和开始菜单创建快捷方式，在右键菜单添加「Open with Atom」，让 Atom 能够在用户从「打开方式」里选取关联程序时可见。

![Atom on Windows](./images/windows.gif)

图 2. Windows 下的 Atom

#### 便携模式

Atom 在 Windows 下有一种便携模式，允许将它自己和 Settings、Packages 和缓存等都放置在可移动设备上，这将使你能很容易地把 Atom 拿到另一台机器使用，不用安装任何东西。
