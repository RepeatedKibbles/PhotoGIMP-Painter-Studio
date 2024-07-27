注意：尽管项目目前功能非常完善，您可能在使用过程中不会遇到任何或仅有轻微的问题，但需要注意的是，我暂时无法实现新功能或分析错误报告。
除此之外，享受 PhotoGIMP Painter Studio 吧！ :)

# 🎨 PhotoGIMP Painter Studio

<img src="./.local/share/icons/hicolor/256x256/apps/photogimp.png" align="right" alt="PhotoGimp 应用图标" title="PhotoGimp 应用图标">

一个为 Adobe Photoshop 用户优化 GIMP 2.10+ 的补丁，包含以下功能：

* 工具组织模仿 Adobe Photoshop 的位置；
* 默认安装新的 Python 过滤器，如“heal selection”；
* 新的启动画面；
* 新的默认设置，最大化画布空间；
* 类似 Photoshop 的快捷键，遵循 Adobe 文档；
* 新图标和自定义 .desktop 文件名称；
* 默认使用系统语言，您仍然可以在设置中更改；
* 画笔以图标形式显示。（适合不同语言的用户）
* 有序排列和清晰分类；
* 选择合适的画笔并更换画笔形状以获得新效果。（避免总是创建新画笔）
* 项目中包含的 SVG 文件（路径）可与画笔一起使用以创建效果线条。

![PhotoGimp Diolinux 启动画面](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/photogimp-diolinux-splash.png)
![GPS Techno Dark 启动画面](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/GPS-2_0--splash-techno-dark.jpg)

# 什么是 GIMP Paint Studio (GPS)？

GPS 是一组画笔和相应的工具预设。工具预设是简单的保存工具选项，这是 GIMP 的一个非常有用的功能。

GPS 的目标是为平面设计师和艺术家提供一个合适的工作环境，使他们从第一次使用 GIMP 开始就能绘画并感到舒适。后来，用户将根据自己的工作流程偏好和对 GIMP 的理解来更改这些设置。

您可以在 [Wiki](https://code.google.com/archive/p/gps-gimp-paint-studio/) 中了解更多关于 GPS 的信息。

感谢使用！祝您绘画愉快！
[Ramón Miranda GPS 拥有者](www.ramonmiranda.com)

# 项目名称
项目名称 = `我的名字缩写` + `GIMP` + `Painter`

- 单词 `Painter` 更好地解释了项目的功能。GIMP 与 Painter 中的 `P` 相邻，因此两个 `P` 被合并。

项目名称是 **SLOS-GIMPainter**

# MyPaintBrushes-GIMP
适用于 GIMP 2.10.x 的 MyPaint-Brushes

![img](https://raw.githubusercontent.com/SenlinOS/databox/master/MyPaint-Brushes-for-GIMP-2.10-By_SenlinOS.jpg)

**[我](https://github.com/SenlinOS) 制作了这些适用于 GIMP 的 MyPaint-Brushes**。

**这些画笔不适用于 MyPaint**，例如在 MyPaint 中的 “002 Frame Line” 将会出现“笔漏”现象。
<br />在 GIMP 2.10 中，按住 Shift 键可以用 “002 Frame Line” 画直线。

其他画笔也已调试，例如 “005 Calligraph” 是一个硬边。
<br />“006 Paint Brush” 在最大压力下绘制时，边缘不会锯齿。

**MyPaint 不需要这些画笔**，它们只是为 GIMP 2.10 设计的。
<br />而且 [我](https://github.com/SenlinOS) 在调试时意外删除了 MyPaint-brushes 的 “.conf” 文件…

# 样式：
有序排列和清晰分类。

## 📷 截图

![PhotoGimp 截图 OSX](./screenshots/osx.png)

## ⚙ 如何安装（使用 Flatpak）

这个包是关于 flatpak 的，但它也包含了可以在任何版本的 GIMP 上使用的“仅文件”（.deb, .rpm, Snap, AppImage, Windows, macOS）。只需检查 GIMP 配置文件的位置。

**在安装后启动并退出 GIMP 后再继续！**

### 准备 Flatpak 环境

*如果您之前通过 .deb, .rpm 等方式安装过 GIMP，请确保删除目录 `$HOME/.config/GIMP`，因为这可能会与 Flatpak 配置文件发生冲突。*

1. 首先，您需要在系统上安装最新的 GIMP [使用 Flatpak](https://flatpak.org/setup/)
2. 通过 AppCenter/包管理器或终端安装 GIMP Flatpak：
   ```flatpak install flathub org.gimp.GIMP```

### 安装 PhotoGIMP Painter Studio

在 [PhotoGIMP-Painter-Studio-master.zip](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/archive/refs/heads/master.zip) 的 .zip 文件中，您会发现三个文件夹（在非 Windows 系统上由于名称以点开头而隐藏）。所有这些文件夹必须解压到您的 `$HOME` 文件夹，如果您已经有旧安装的相同文件，请覆盖它们。

文件包含以下目录：

* `.icons`（其中有一个新的 PhotoGIMP 图标）
* `.local`（其中包含个性化的 .desktop 文件）
* `.var`（其中包含适用于 GIMP 2.10+ 的 flatpak 补丁自定义）

如果您只想要 PhotoGIMP 自定义而不更改原始 GIMP 图标和名称，只需将 ```.var``` 文件夹解压到您的主目录。

- 编辑 -> 首选项 ->（文件夹 -> MyPaint 画笔）。
- 单击 [添加新文件夹] 按钮以打开 [SLOS_MPB] 目录。
- 重启 GIMP。

## ⚙ 如何安装（其他）

由于它只是文件，您只需将此包中的特定文件夹 `/.var/app/org.gimp.GIMP/config/GIMP/2.10` 中的所有文件复制到各系统上的 GIMP 配置文件夹中，覆盖现有文件即可。

**在安装后启动并退出 GIMP 后再继续！**

新图标需要手动设置。

### Ubuntu Snap

配置文件夹：`$HOME/snap/gimp/47/.config/GIMP/2.10/`

### 其他 Linux 或 Unix 类系统（.deb, .rpm 等）

配置文件夹：`$HOME/.config/GIMP/2.10/`

### macOS

配置文件夹：`"$HOME/Library/Application Support/GIMP/2.10/"`

* [Davies Media Design 在 macOS 上的视频教程](https://youtu.be/5nXhtaGQs9U)

### Mac OS 简易安装程序（作者：[@MatthijsKamstra](https://github.com/MatthijsKamstra)）

> 需要先安装 Gimp（[brew](https://formulae.brew.sh/cask/gimp) 或 [其他方式](https://www.gimp.org/downloads/)）

##### 运行 bash 安装脚本

您可以[下载](https://raw.githubusercontent.com/MatthijsKamstra/Mac-setup/master/install/photogimp_osx.sh)并运行 bash 脚本：

```bash
cd /path/to/download/folder
sh photogimp_osx.sh
```

### Windows

* 下载文件 [PhotoGIMP-Painter-Studio-master.zip](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/archive/refs/heads/master.zip)
* 从 ZIP 中访问路径 `.var\app\org.gimp.GIMP\config\GIMP\2.10`，将文件复制到路径 `%APPDATA%\GIMP\2.10`
* [Davies Media Design 在 Windows 上的视频教程](https://youtu.be/57DNUsf4A-0)

# 显示对话框
打开窗口菜单：可停靠的对话框 -> 工具预设，您可以看到 SLOS-GIMPainter。

- 单击工具预设对话框右上角的小三角按钮，然后单击 `网格视图`。
- 单击工具预设对话框右上角的小三角按钮到 `预览大小` 并选择 `大`。
- 选择工具预设对话框顶部的 `SLOS` 标签以隐藏内置预设。

	**设置后，在菜单中，编辑 -> 首选项 -> 界面（窗口管理），按照截图保存设置，然后单击确定完成。**

	![(窗口管理](https://raw.githubusercontent.com/SenlinOS/databox/master/SLOS-GIMPainter-Installation/wmment.jpg)

## 致谢

* 没有 GIMP 团队的努力，这个项目是不可能实现的。
* 新启动画面的照片来自 [Isabella Mariana](https://www.pexels.com/pt-br/@isabella-mariana-1022505)
* 非常感谢所有在 [Twitch](https://twitch.tv/Diolinux) 和 [YouTube](https://youtube.com/Diolinux) 上支持 Diolinux 的人们。
*

 [GIMP Resynthesizer 插件套件](https://www.logarithmic.net/pfh/resynthesizer) 最初由 [Paul Harrison](https://logarithmic.net/pfh/) 开发，现在由 [Lloyd Konneker (也称为 bootchk)](https://github.com/bootchk) 维护。
* [GIMP Paint Studio](https://code.google.com/archive/p/gps-gimp-paint-studio/) 最初由 [Ramon Miranda](https://www.ramonmiranda.com/) 开发，现在由 [PkGam](https://www.deviantart.com/pkgam/art/GIMP-Paint-Studio-2-0-2-1-Port-to-GIMP-2-10-850663044) 从 GIMP 2.8 移植到 2.10+。
* [GIMP 2.10 工具预设修复](https://www.deviantart.com/pkgam/art/GIMP-2-10-Tool-Preset-Fixes-749387099) 由 [PkGam](https://www.deviantart.com/pkgam) 开发。
* [SLOS-GIMPainter](https://github.com/SenlinOS/SLOS-GIMPainter) 由 [SenlinOS](https://github.com/SenlinOS) 开发。
* [MyPaintBrushes-GIMP](https://github.com/SenlinOS/MyPaintBrushes-GIMP) 由 [SenlinOS](https://github.com/SenlinOS) 开发。

# 许可证
项目遵循 GPL-3.0、GPL-2.0、MIT、CC BY-SA 3.0 和 CC0 许可证。有关更多信息，请参见 LICENSE 文件。

**- GNU 通用公共许可证 (GPL):**
* gps-gimp-paint-studio ([GPL-2.0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=GPL-2.0-3-ov-file))
* PhotoGIMP ([GPL-3.0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=GPL-3.0-4-ov-file))

**- 麻省理工学院 (MIT):**
* [SLOS-GIMPainter](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=MIT-5-ov-file)

**- 创作共用 (CC):**
* MyPaintBrushes-GIMP ([CC0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=CC0-1.0-1-ov-file))
* gps-gimp-paint-studio ([CC BY-SA 3.0 (内容许可证)](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=License-2-ov-file))

---

![视频演示图片](https://raw.githubusercontent.com/SenlinOS/databox/master/video-demo-img.jpg)

**文字描述：**

- 关于线稿，请查看文字描述：[这里](https://github.com/SenlinOS/databox/blob/master/For-Line-Art_SLOS-GIMPainter.md)。
- 手动保存临时预设，文字+视频：[这里](https://github.com/SenlinOS/databox/blob/master/manually-save-temporary-presets.md)。

**其他提示：**

- GNU/Linux(X11) 软件变为描图纸，视频：[这里](https://youtu.be/ArHPMmIMsq8)。

- 如何在 GIMP 中制作透视线，视频：[这里](https://youtu.be/gIp5I0fXdlM)。

## 贡献者 (PhotoGIMP)
<a align="center" href="https://github.com/Diolinux/PhotoGIMP/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Diolinux/PhotoGIMP" />
</a>

## 补丁说明
-  [查看葡萄牙语发行说明](https://diolinux.com.br/2020/06/photogimp-2020.html)
