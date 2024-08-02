注意：虽然该项目本身功能非常强大，您可能可以毫无问题地使用它，但需要注意的是，[我](https://github.com/Diolinux) 目前无法实现新功能或分析错误报告。
除此之外，请尽情享受 PhotoGIMP Painter Studio！:)

# 🎨 PhotoGIMP Painter Studio

<img src="./.local/share/icons/hicolor/256x256/apps/photogimp.png" align="right" alt="PhotoGimp 应用程序图标" title="PhotoGimp 应用程序图标">

针对 Adob​​e Photoshop 用户优化 GIMP 2.10+ 的补丁，包括以下功能：

* 工具组织以模仿 Adob​​e Photoshop 的位置；
* 默认安装新的 Python 过滤器，例如“修复选择”；
* 新的启动画面
* 新的默认设置以最大化画布上的空间；
* 快捷键类似于 Windows 版 Photoshop 中的快捷键，遵循 Adob​​e 的文档；
* 来自自定义 .desktop 文件的新图标和名称。
* 现在默认使用系统语言，您仍可以在设置中更改。
* 画笔显示为图标。（适合不同语言的用户）
* 有序排列，分类清晰。
* 选择合适的画笔并替换画笔形状以获得新效果。（避免总是创建新画笔）
* 项目中包含的 SVG 文件（路径）可与画笔一起使用以创建效果线。

![PhotoGimp Diolinux Splash Art](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/photogimp-diolinux-splash.png)
![GPS Techno Dark Splash Art](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/GPS-2_0--splash-techno-dark.jpg)

# 什么是 GIMP Paint Studio (GPS)？

GPS 是画笔和随附工具预设的集合。工具预设是一种简单保存的工具选项，是 GIMP 的非常有用的功能。

GPS 的目标是为图形设计师和艺术家提供适当的工作环境，让他们从第一次使用 GIMP 开始绘画并感到舒适。稍后，用户将根据自己的工作流程偏好和对 GIMP 的理解更改这些设置。

您可以在 [WIki](https://code.google.com/archive/p/gps-gimp-paint-studio/) 中了解有关 GPS 的更多信息

感谢您使用它！祝您绘画愉快！
[Ramón Miranda GPS 所有者](www.ramonmiranda.com)

# 项目名称
项目名称 = `我的名字缩写` + `GIMP` + `Painter`

- `Painter` 一词可以更好地解释项目的功能。GIMP 与 Painter 中的 `P` 相邻，因此将两个 `P` 合并。

项目名称为**SLOS-GIMPainter**

# MyPaintBrushes-GIMP
MyPaint-Brushes for GIMP 2.10.x

![img](https://raw.githubusercontent.com/SenlinOS/databox/master/MyPaint-Brushes-for-GIMP-2.10-By_SenlinOS.jpg)

**[我](https://github.com/SenlinOS)为 GIMP 制作了这些 MyPaint-Brushes**。

**这些笔刷不适合 MyPaint**，比如“002 Frame Line”在 MyPaint 中会出现“漏笔”现象。
<br />在 GIMP 2.10 中，按住 Shift 键“002 Frame Line”可以画直线。

其他笔刷也调试过了，比如“005 Calligraph”是硬边。
<br />“006 Paint Brush” 以最大压力绘制，边缘不会参差不齐。

**MyPaint 不需要这些画笔**，它只是为 GIMP 2.10 设计的。
<br />而且 [我](https://github.com/SenlinOS) 在调试时不小心删除了 MyPaint-brushes “.conf” 文件……

# 风格：
有序排列，分类清晰。

## 📷 截图

![PhotoGimp Screenshot OSX](./screenshots/osx.png)

## ⚙ 如何安装（使用 Flatpak）

这个包是关于 flatpak 的，但它还包含“仅文件”，您可以在任何版本的 GIMP（.deb、.rpm、Snap、AppImage、Windows、macOS）上使用。只需检查 GIMP 配置文件的位置。

**安装后，请启动并退出 GIMP，然后再继续！**

### 准备 Flatpak 环境

*如果您之前已通过 .deb、.rpm 等安装了 GIMP，请确保删除目录 `$HOME/.config/GIMP`，因为这可能会导致与 Flatpak 配置文件发生冲突。*

1. 首先，您需要在系统上安装最新的 GIMP [使用 Flatpak](https://flatpak.org/setup/)
2. 通过 AppCenter/Package Manager 或终端安装 GIMP Flatpak：
```flatpak install flathub org.gimp.GIMP```

### 安装 PhotoGIMP Painter Studio

在 [PhotoGIMP-Painter-Studio-master.zip](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/archive/refs/heads/master.zip) 的 .zip 文件中，您会找到三个文件夹（在非 Windows 系统上隐藏，因为它们的名称以点开头）。所有这些文件夹都必须提取到您的 `$HOME` 文件夹中，如果您已经拥有旧安装中的相同文件，则将覆盖所有内容。

该文件包含以下目录：

* `.icons`（包含新的 PhotoGIMP 图标）
* `.local`（包含个性化的 .desktop 文件）
* `.var`（包含 GIMP 2.10+ 的 flatpak 补丁自定义）

如果您只想要 PhotoGIMP 自定义而不更改原始 GIMP 图标及其名称，只需将 ```.var`` 文件夹提取到您的主目录即可。

- 编辑 -> 首选项 ->(文件夹 -> MyPaint 画笔)。
- 单击 [添加新文件夹] 按钮打开 [SLOS_MPB] 目录。
- 重新启动 GIMP。

## ⚙ 如何安装（其他）

由于它只是文件，因此您唯一需要做的就是将此包 `/.var/app/org.gimp.GIMP/config/GIMP/2.10` 中特定文件夹中的所有文件复制到每个特定系统上的 GIMP 配置文件夹中，覆盖现有的文件。

**安装后，请启动并退出 GIMP，然后再继续！**

需要手动设置新图标。

### Ubuntu Snap

配置文件夹：`$HOME/snap/gimp/47/.config/GIMP/2.10/`

### 其他 Linux 或类 Unix 系统（.deb、.rpm 等）

配置文件夹：`$HOME/.config/GIMP/2.10/`

### macOS

配置文件夹：`"$HOME/Library/Application Support/GIMP/2.10/"`

* [Davies Media Design 在 macOS 上的视频教程](https://youtu.be/5nXhtaGQs9U)

### Mac OS Easy Installer（由 [@MatthijsKamstra](https://github.com/MatthijsKamstra) 制作）

> 需要安装 Gimp ([brew](https://formulae.brew.sh/cask/gimp) 或[其他](https://www.gimp.org/downloads/))

##### 运行 bash 如何

您可以[down](https://raw.githubusercontent.com/MatthijsKamstra/Mac-setup/master/install/photogimp_osx.sh)并运行 bash 脚本：

```bash
cd /path/to/download/folder
sh photogimp_osx.sh
```

### Windows

* 下载文件 [PhotoGIMP-Painter-Studio-master.zip](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/archive/refs/heads/master.zip)
* 从 ZIP 访问路径 `.var\app\org.gimp.GIMP\config\GIMP\2.10`，将文件复制到路径 `%APPDATA%\GIMP\2.10`
* [Davies Media Design 的视频教程Windows](https://youtu.be/57DNUsf4A-0)

# 显示对话框
打开窗口菜单：可停靠对话框 -> 工具预设，即可看到 SLOS-GIMPainter。

- 点击工具预设对话框右上角的小三角按钮，点击“以网格形式查看”。
- 点击工具预设对话框右上角的小三角按钮“预览尺寸”，选择“大”。
- 选择工具预设对话框顶部的“SLOS”选项卡，隐藏内置预设。

**设置完成后，在菜单中，编辑 -> 首选项 -> 界面（窗口管理），保存设置，如截图所示，点击确定即可完成。**

![(窗口管理](https://raw.githubusercontent.com/SenlinOS/databox/master/SLOS-GIMPainter-Installation/wmment.jpg)

## 致谢

* 如果没有出色的 GIMP 团队，这个项目不可能实现。
* 新 Splash 中的照片来自 [Isabella Mariana](https://www.pexels.com/pt-br/@isabella-mariana-1022505)
* 非常感谢 Diolinux 在 [Twitch](https://twitch.tv/Diolinux) 和 [YouTube](https://youtube.com/Diolinux) 上的所有支持者。
* [GIMP Resynthesizer 插件Suite](https://www.logarithmic.net/pfh/resynthesizer) 最初由 [Paul Harrison](https://logarithmic.net/pfh/) 开发，现在由 [Lloyd Konneker (也称为 bootchk)](https://github.com/bootchk) 接管 [维护](https://github.com/bootchk/resynthesizer)
* [GIMP Paint Studio](https://code.google.com/archive/p/gps-gimp-paint-studio/) 最初由 [Ramon Miranda](https://www.ramonmiranda.com/) 开发，现在由 [移植](https://www.deviantart.com/pkgam/art/GIMP-Paint-Studio-2-0-2-1-Port-to-GIMP-2-10-850663044) 从 GIMP 2.8 升级到 2.10+ [PkGam](https://www.deviantart.com/pkgam)
* [GIMP 2.10 工具预设修复](https://www.deviantart.com/pkgam/art/GIMP-2-10-Tool-Preset-Fixes-749387099) 由 [PkGam](https://www.deviantart.com/pkgam) 开发
* [SLOS-GIMPainter](https://github.com/SenlinOS/SLOS-GIMPainter) 由 [SenlinOS](https://github.com/SenlinOS) 开发
* [MyPaintBrushes-GIMP](https://github.com/SenlinOS/MyPaintBrushes-GIMP) 由 [SenlinOS](https://github.com/SenlinOS) 开发

# 许可证
该项目遵循 GPL-3.0、GPL-2.0、MIT、CC BY-SA 3.0 和 CC0 许可证。有关更多信息，请参阅许可证文件。

**- GNU 通用公共许可证 (GPL)：**
* gps-gimp-paint-studio ([GPL-2.0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=GPL-2.0-3-ov-file))
* PhotoGIMP ([GPL-3.0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=GPL-3.0-4-ov-file))

**- 麻省理工学院 (MIT)：**
* [SLOS-GIMPainter](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=MIT-5-ov-file)

**- 知识共享许可证 (CC)：**
* MyPaintBrushes-GIMP ([CC0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=CC0-1.0-1-ov-file))
* gps-gimp-paint-studio ([CC BY-SA 3.0（内容许可）](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=License-2-ov-file))

---

![Vimg](https://raw.githubusercontent.com/SenlinOS/databox/master/video-demo-img.jpg)

**关于详细的讲解，请看我的视频演示：**
<br />(无声 / 字幕)

[在B站的演示视频合集](https://space.bilibili.com/14824534/channel/seriesdetail?sid=1169812&ctype=0)。

对于线艺术，请查看文字说明：[这里](https://github.com/SenlinOS/databox/blob/master/For-Line-Art_SLOS-GIMPainter.md)。

手动保存临时预设：[这里](https://senlinos.github.io/post/manually-save-temporary-presets/) 和 [这里](https://t.bilibili.com/519640070146405433?tab=2)。

**其他技巧：**

- GNU/Linux(X11)中将软件变成描图纸：[我的B站视频](https://www.bilibili.com/video/BV18R4y1j7g6)。

- GIMP中怎样制作透视线：[我的B站视频](https://www.bilibili.com/video/BV1AS4y1V7AB)。
