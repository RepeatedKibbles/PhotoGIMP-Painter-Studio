NOTE: Although the project is very functional as it is and you probably can use it with minor to no problems, it's important to notice that [I'm](https://github.com/Diolinux) note not able to implement new features or analyze bug reports for now.
Other than that, enjoy PhotoGIMP Painter Studio! :)

# 🎨 PhotoGIMP Painter Studio

<img src="./.local/share/icons/hicolor/256x256/apps/photogimp.png" align="right" alt="PhotoGimp application icon" title="PhotoGimp application icon">

A patch for optimizing GIMP 2.10+ for Adobe Photoshop users, including features like:

* Tool organization to mimic the position of Adobe Photoshop;
* New Python filters installed by default, such as "heal selection";
* New Splash Screen
* New default settings to maximize space on the canvas;
* Shortcuts similar to the ones in Photoshop for Windows, following Adobe’s Documentation;
* New icon and Name from custom .desktop file.
* System Language is now used by default, you can still change in settings if you want.
* Brushes are displayed as Icons. (Suitable for users of different languages)
* Orderly arrangement and clear classification.
* Choose a suitable Brush and replace the brush shape to get a new effect. (Avoid always creating new brushes)
* SVG files (Paths) included with the project can be used with brushes to create effect lines.

![PhotoGimp Diolinux Splash Art](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/photogimp-diolinux-splash.png)
![GPS Techno Dark Splash Art](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/GPS-2_0--splash-techno-dark.jpg)

# What is GIMP Paint Studio (GPS)?

GPS is a collection of brushes and accompanying tool presets. Tool presets are a simply saved tool options, highly useful feature of the GIMP.

The goal of GPS is to provide an adequate working environment for graphic designers and artists to begin to paint and feel comfortable with GIMP from their first use. Later the user will change these settings based on his own workflow preferences and understanding of GIMP.

You can learn more about GPS in the [WIki](https://code.google.com/archive/p/gps-gimp-paint-studio/)

Thanks for using it! happy painting!
[Ramón Miranda GPS owner](www.ramonmiranda.com)

# Project Name
The project name = `My Name Abbreviation` + `GIMP` + `Painter`

- The word `Painter` to better explain the function of the project. GIMP is adjacent to the `P` in Painter, so the two `P` are merged.

The name of the project is **SLOS-GIMPainter**

# MyPaintBrushes-GIMP
MyPaint-Brushes for GIMP 2.10.x

![img](https://raw.githubusercontent.com/SenlinOS/databox/master/MyPaint-Brushes-for-GIMP-2.10-By_SenlinOS.jpg)

**[I](https://github.com/SenlinOS) made these MyPaint-Brushes for GIMP**.

**This brushes is not suitable for MyPaint**, such as “002 Frame Line” in MyPaint will “pen leaking” phenomenon.
<br />In GIMP 2.10, hold down the Shift key “002 Frame Line” can draw a straight line.

Other brushes have also been debugged, such as “005 Calligraph” is a hard edge.
<br />“006 Paint Brush” to draw at maximum pressure, the edges will not jagged.

**MyPaint doesn't need these brushes**, it is just designed for GIMP 2.10.
<br />And [I](https://github.com/SenlinOS) accidentally deleted MyPaint-brushes “.conf” file when debugging…

# Style:
Orderly arrangement and clear classification.

## 📷 Screenshots

![PhotoGimp Screenshot OSX](./screenshots/osx.png)

## ⚙ How to Install (using Flatpak)

This package is all about flatpak, but it also contains "just files" that you can use on any version of GIMP (.deb, .rpm, Snap, AppImage, Windows, macOS). Just check the location of the GIMP configuration files.

**Start and quit GIMP after you installed before you continue!**

### Prepare the Flatpak environment

*If you have previously had GIMP installed via .deb, .rpm, etc., please ensure you delete the directory `$HOME/.config/GIMP`, as this may cause conflicts with the Flatpak config files.*

1. First of all, you need to have the latest GIMP installed on your system [using Flatpak](https://flatpak.org/setup/)
2. Install GIMP Flatpak through your AppCenter/Package Manager or terminal:
   ```flatpak install flathub org.gimp.GIMP```

### Install PhotoGIMP Painter Studio

Inside the .zip file from the [PhotoGIMP-Painter-Studio-master.zip](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/archive/refs/heads/master.zip) you’ll find three folders (hidden on non-Windows systems as their names begin with a dot). All of these folders have to be extracted to your `$HOME` folder, overwriting everything if you already have the same files from an older installation.

The file contains these directories:

* `.icons` (which has a new PhotoGIMP icon)
* `.local` (which contains the personalized .desktop file)
* `.var` (which contains the flatpak patch customization for GIMP 2.10+)

If you just want the PhotoGIMP customization without changing the original GIMP icon and its name, just extract only the ```.var``` folder to your home directory.

- Edit -> Preferences ->(Folders -> MyPaint Brushes).
- Click on the [Add a new folder] button to open the [SLOS_MPB] directory.
- Restart GIMP.

## ⚙ How to Install (others)

Since it’s just files, the only thing you need to do is to copy all the files that reside on a particular folder from this package `/.var/app/org.gimp.GIMP/config/GIMP/2.10` to your GIMP’s configuration folder on each particular system, overriding the existent ones.

**Start and quit GIMP after you installed before you continue!**

The new icon needs to be set manually.

### Ubuntu Snap

Configuration folder: `$HOME/snap/gimp/47/.config/GIMP/2.10/`

### Other Linux or Unix(-like) systems (.deb, .rpm, etc.)

Configuration folder: `$HOME/.config/GIMP/2.10/`

### macOS

Configuration folder: `"$HOME/Library/Application Support/GIMP/2.10/"`

* [Video Tutorial by Davies Media Design on macOS](https://youtu.be/5nXhtaGQs9U)

### Mac OS Easy Installer (made by: [@MatthijsKamstra](https://github.com/MatthijsKamstra))

> Gimp needs to be installed ([brew](https://formulae.brew.sh/cask/gimp) or [otherwise](https://www.gimp.org/downloads/))

<<<<<<< HEAD
=======
What will the [bash](https://raw.githubusercontent.com/MatthijsKamstra/Mac-setup/master/install/photogimp_osx.sh) script do?

* Download `Flatpak.zip` and copies the files to the Gimp folder
* Creates an OSX PhotoGimp icon
* Copies icon to Gimp folder
* Cleans up all files generated/downloaded

>>>>>>> 94ab263bec885f5236e7f4548dc51fbac4e21685
##### Run bash how to

you can [down](https://raw.githubusercontent.com/MatthijsKamstra/Mac-setup/master/install/photogimp_osx.sh) and run the bash script:

```bash
cd /path/to/download/folder
sh photogimp_osx.sh
```

### Windows

* Download the file [PhotoGIMP-Painter-Studio-master.zip](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/archive/refs/heads/master.zip)
* Access the path `.var\app\org.gimp.GIMP\config\GIMP\2.10` from the ZIP, copy the files to the path `%APPDATA%\GIMP\2.10`
* [Video Tutorial by Davies Media Design on Windows](https://youtu.be/57DNUsf4A-0)

# Show Dialog
Open the Window menu: Dockable Dialogs -> Tool Presets, and you can see SLOS-GIMPainter.

- Click the small triangle button on the upper right of the Tool Presets dialog, and click to `View as Grid`.
- Click the small triangle button on the upper right of the Tool Presets dialog to `Preview Size` and select the `Large`.
- Select the `SLOS` tab at the top of Tool Presets dialog to hide the built-in presets.

	**After setting, in the menu, Edit -> Preferences -> Interface(Window Management), save the settings as shown in the screenshot, and click OK to finish.**

	![(Window Management](https://raw.githubusercontent.com/SenlinOS/databox/master/SLOS-GIMPainter-Installation/wmment.jpg)

## Credits

* This project would not be possible without the amazing GIMP team.
* The Photo in the new Splash is from [Isabella Mariana](https://www.pexels.com/pt-br/@isabella-mariana-1022505)
* A BIG thanks to all Diolinux’s supporters on [Twitch](https://twitch.tv/Diolinux) and [YouTube](https://youtube.com/Diolinux).
* [GIMP Resynthesizer Plugin Suite](https://www.logarithmic.net/pfh/resynthesizer) was originally developed by [Paul Harrison](https://logarithmic.net/pfh/) and now taken over [maintenance](https://github.com/bootchk/resynthesizer) by [Lloyd Konneker (also known as, bootchk)](https://github.com/bootchk)
* [GIMP Paint Studio](https://code.google.com/archive/p/gps-gimp-paint-studio/) was originally developed by [Ramon Miranda](https://www.ramonmiranda.com/) and now [ported](https://www.deviantart.com/pkgam/art/GIMP-Paint-Studio-2-0-2-1-Port-to-GIMP-2-10-850663044) from GIMP 2.8 to 2.10+ by [PkGam](https://www.deviantart.com/pkgam)
* [GIMP 2.10 Tool Preset Fixes](https://www.deviantart.com/pkgam/art/GIMP-2-10-Tool-Preset-Fixes-749387099) developed by [PkGam](https://www.deviantart.com/pkgam)
* [SLOS-GIMPainter](https://github.com/SenlinOS/SLOS-GIMPainter) developed by [SenlinOS](https://github.com/SenlinOS)
* [MyPaintBrushes-GIMP](https://github.com/SenlinOS/MyPaintBrushes-GIMP) developed by [SenlinOS](https://github.com/SenlinOS)

# License
The Project is under an GPL-3.0, GPL-2.0, MIT, CC BY-SA 3.0, and CC0 License. See the LICENSE file for more information.

**- GNU General Public (GPL):**
* gps-gimp-paint-studio ([GPL-2.0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=GPL-2.0-3-ov-file))
* PhotoGIMP ([GPL-3.0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=GPL-3.0-4-ov-file))

**- Massachusetts Institute of Technology (MIT):**
* [SLOS-GIMPainter](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=MIT-5-ov-file)

**- Creative Commons (CC):**
* MyPaintBrushes-GIMP ([CC0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=CC0-1.0-1-ov-file))
* gps-gimp-paint-studio ([CC BY-SA 3.0 (License for Contents)](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=License-2-ov-file))

---

![Vimg](https://raw.githubusercontent.com/SenlinOS/databox/master/video-demo-img.jpg)

**Text Description:**

- For Line Art, please check the text description: [Here](https://github.com/SenlinOS/databox/blob/master/For-Line-Art_SLOS-GIMPainter.md).
- Manually save temporary presets, the text+video: [Here](https://github.com/SenlinOS/databox/blob/master/manually-save-temporary-presets.md).

**Other Tips:**

- GNU/Linux(X11) software becomes tracing paper, video: [Here](https://youtu.be/ArHPMmIMsq8).

- How to make perspective lines in GIMP, video: [Here](https://youtu.be/gIp5I0fXdlM).

## Contributors (PhotoGIMP)
<a align="center" href="https://github.com/Diolinux/PhotoGIMP/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Diolinux/PhotoGIMP" />
</a>

## Patch Notes
-  [Veja as Notas de Lançamento em Português](https://diolinux.com.br/2020/06/photogimp-2020.html)
