UWAGA: Chociaż projekt jest bardzo funkcjonalny i prawdopodobnie można go używać z niewielkimi lub żadnymi problemami, ważne jest, aby zauważyć, że [I am](https://github.com/Diolinux) nie jest w stanie wdrożyć nowych funkcji ani analizować raportów o błędach na razie.
Poza tym, ciesz się PhotoGIMP Painter Studio! :)

# 🎨 PhotoGIMP Painter Studio

<img src="./.local/share/icons/hicolor/256x256/apps/photogimp.png" align="right" alt="PhotoGimp application icon" title="PhotoGimp application icon">

Łatka optymalizująca GIMP 2.10+ dla użytkowników Adobe Photoshop, zawierająca takie funkcje jak:

* Organizacja narzędzi w celu naśladowania położenia Adobe Photoshop;
* Nowe filtry Pythona instalowane domyślnie, takie jak „heal selection”;
* Nowy ekran powitalny
* Nowe ustawienia domyślne w celu maksymalizacji przestrzeni na płótnie;
* Skróty podobne do tych w Photoshopie dla Windows, zgodnie z dokumentacją Adobe;
* Nowa ikona i nazwa z niestandardowego pliku .desktop.
* Język systemowy jest teraz używany domyślnie, nadal możesz zmienić w ustawieniach, jeśli chcesz.
* Pędzle są wyświetlane jako ikony. (Odpowiednie dla użytkowników różnych języków)
* Uporządkowane rozmieszczenie i przejrzysta klasyfikacja.
* Wybierz odpowiedni pędzel i zmień kształt pędzla, aby uzyskać nowy efekt. (Unikaj ciągłego tworzenia nowych pędzli)
* Pliki SVG (ścieżki) dołączone do projektu mogą być używane z pędzlami w celu tworzenia linii efektów.

![PhotoGimp Diolinux Splash Art](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/photogimp-diolinux-splash.png)
![GPS Techno Dark Splash Art](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/GPS-2_0--splash-techno-dark.jpg)

# Czym jest GIMP Paint Studio (GPS)?

GPS to zbiór pędzli i towarzyszących im ustawień wstępnych narzędzi. Ustawienia wstępne narzędzi to po prostu zapisane opcje narzędzi, bardzo przydatna funkcja GIMP.

Celem GPS jest zapewnienie odpowiedniego środowiska pracy dla projektantów graficznych i artystów, aby mogli zacząć malować i czuć się komfortowo z GIMP od pierwszego użycia. Później użytkownik zmieni te ustawienia na podstawie własnych preferencji przepływu pracy i zrozumienia GIMP.

Możesz dowiedzieć się więcej o GPS w [WIki](https://code.google.com/archive/p/gps-gimp-paint-studio/)

Dzięki za korzystanie! Miłego malowania!
[Ramón Miranda GPS owner](www.ramonmiranda.com)

# Nazwa projektu
Nazwa projektu = `My Name Abbreviation` + `GIMP` + `Painter`

- Słowo `Painter`, aby lepiej wyjaśnić funkcję projektu. GIMP sąsiaduje z `P` w Painter, więc dwa `P` są połączone.

Nazwa projektu to **SLOS-GIMPainter**

# MyPaintBrushes-GIMP
MyPaint-Brushes dla GIMP 2.10.x

![img](https://raw.githubusercontent.com/SenlinOS/databox/master/MyPaint-Brushes-for-GIMP-2.10-By_SenlinOS.jpg)

**[I](https://github.com/SenlinOS) stworzył te MyPaint-Brushes dla GIMP**.

**Te pędzle nie nadają się do MyPaint**, takie jak „002 Frame Line” w MyPaint będą powodować zjawisko „przeciekania pióra”.
<br /> W GIMP 2.10 przytrzymaj klawisz Shift „002 Frame Line” aby narysować prostą linię.

Inne pędzle również zostały debugowane, takie jak „005 Calligraph” to twarda krawędź.
<br />„006 Paint Brush” do rysowania z maksymalnym naciskiem, krawędzie nie będą postrzępione.

**MyPaint nie potrzebuje tych pędzli**, jest przeznaczony tylko dla GIMP 2.10.
<br /> I [I](https://github.com/SenlinOS) przypadkowo usunąłem plik „.conf” MyPaint-brushes podczas debugowania…

# Styl:
Uporządkowany układ i przejrzysta klasyfikacja.

## 📷 Zrzuty ekranu

![Zrzut ekranu PhotoGimp OSX](./screenshots/osx.png)

## ⚙ Jak zainstalować (używając Flatpak)

Ten pakiet dotyczy wyłącznie flatpak, ale zawiera również „tylko pliki”, których można używać w dowolnej wersji GIMP (.deb, .rpm, Snap, AppImage, Windows, macOS). Wystarczy sprawdzić lokalizację plików konfiguracyjnych GIMP.

**Uruchom i zamknij GIMP po zainstalowaniu, zanim przejdziesz dalej!**

### Przygotuj środowisko Flatpak

*Jeśli wcześniej zainstalowałeś GIMP za pomocą .deb, .rpm itp., upewnij się, że usunąłeś katalog `$HOME/.config/GIMP`, ponieważ może to spowodować konflikty z plikami konfiguracyjnymi Flatpak.*

1. Przede wszystkim musisz mieć zainstalowaną najnowszą wersję GIMP w swoim systemie [za pomocą Flatpak](https://flatpak.org/setup/)
2. Zainstaluj GIMP Flatpak za pomocą AppCenter/Package Manager lub terminala:
```flatpak install flathub org.gimp.GIMP```

### Zainstaluj PhotoGIMP Painter Studio

Wewnątrz pliku .zip z [PhotoGIMP-Painter-Studio-master.zip](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/archive/refs/heads/master.zip) znajdziesz trzy foldery (ukryte w systemach innych niż Windows, ponieważ ich nazwy zaczynają się od kropki). Wszystkie te foldery muszą zostać wypakowane do folderu `$HOME`, nadpisując wszystko, jeśli masz już te same pliki ze starszej instalacji.

Plik zawiera następujące katalogi:

* `.icons` (który ma nową ikonę PhotoGIMP)
* `.local` (który zawiera spersonalizowany plik .desktop)
* `.var` (który zawiera dostosowanie poprawki flatpak dla GIMP 2.10+)

Jeśli chcesz tylko dostosować PhotoGIMP bez zmiany oryginalnej ikony GIMP i jej nazwy, po prostu wypakuj tylko folder ```.var``` do swojego katalogu domowego.

- Edycja -> Preferencje ->(Foldery -> Moje pędzle malarskie).
- Kliknij przycisk [Dodaj nowy folder], aby otworzyć katalog [SLOS_MPB].
- Uruchom ponownie program GIMP.

## ⚙ Jak zainstalować (inne)

Ponieważ są to tylko pliki, jedyne, co musisz zrobić, to skopiować wszystkie pliki znajdujące się w określonym folderze z tego pakietu `/.var/app/org.gimp.GIMP/config/GIMP/2.10` do folderu konfiguracyjnego programu GIMP w każdym konkretnym systemie, zastępując istniejące pliki.

**Uruchom i zamknij program GIMP po zainstalowaniu, zanim przejdziesz dalej!**

Nowa ikona musi zostać ustawiona ręcznie.

### Ubuntu Snap

Folder konfiguracyjny: `$HOME/snap/gimp/47/.config/GIMP/2.10/`

### Inne systemy Linux lub Unix(-like) (.deb, .rpm, itd.)

Folder konfiguracyjny: `$HOME/.config/GIMP/2.10/`

### macOS

Folder konfiguracyjny: `"$HOME/Library/Application Support/GIMP/2.10/"`

* [Samouczek wideo autorstwa Davies Media Design na macOS](https://youtu.be/5nXhtaGQs9U)

### Mac OS Easy Installer (wykonany przez: [@MatthijsKamstra](https://github.com/MatthijsKamstra))

> Gimp musi zostać zainstalowany ([brew](https://formulae.brew.sh/cask/gimp) lub [inaczej](https://www.gimp.org/downloads/))

##### Uruchom bash jak

możesz [download](https://raw.githubusercontent.com/MatthijsKamstra/Mac-setup/master/install/photogimp_osx.sh) i uruchomić skrypt bash:

```bash
cd /path/to/download/folder
sh photogimp_osx.sh
```

### Windows

* Pobierz plik [PhotoGIMP-Painter-Studio-master.zip](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/archive/refs/heads/master.zip)
* Uzyskaj dostęp do ścieżki `.var\app\org.gimp.GIMP\config\GIMP\2.10` z ZIP, skopiuj pliki do ścieżki `%APPDATA%\GIMP\2.10`
* [Samouczek wideo autorstwa Davies Media Design na Windows](https://youtu.be/57DNUsf4A-0)

# Pokaż okno dialogowe
Otwórz menu Okno: Dockable Dialogs -> Tool Presets, a zobaczysz SLOS-GIMPainter.

- Kliknij mały trójkątny przycisk w prawym górnym rogu okna dialogowego Tool Presets i kliknij `View as Grid`.
- Kliknij mały trójkątny przycisk w prawym górnym rogu okna dialogowego Tool Presets, aby `Preview Size` i wybierz `Large`.
- Wybierz kartę `SLOS` u góry okna dialogowego Tool Presets, aby ukryć wbudowane ustawienia wstępne.

**Po ustawieniu w menu Edycja -> Preferencje -> Interfejs (Zarządzanie oknami), zapisz ustawienia, jak pokazano na zrzucie ekranu i kliknij OK, aby zakończyć.**

![(Zarządzanie oknami](https://raw.githubusercontent.com/SenlinOS/databox/master/SLOS-GIMPainter-Installation/wmment.jpg)

## Podziękowania

* Ten projekt nie byłby możliwy bez niesamowitego zespołu GIMP.
* Zdjęcie w nowym Splash jest autorstwa [Isabelli Mariany](https://www.pexels.com/pt-br/@isabella-mariana-1022505)
* WIELKIE podziękowania dla wszystkich zwolenników Diolinux na [Twitchu](https://twitch.tv/Diolinux) i [YouTube](https://youtube.com/Diolinux).
* [Wtyczka GIMP Resynthesizer Pakiet](https://www.logarithmic.net/pfh/resynthesizer) został pierwotnie opracowany przez [Paula Harrisona](https://logarithmic.net/pfh/), a obecnie przejął [opiekę](https://github.com/bootchk/resynthesizer) [Lloyd Konneker (znany również jako bootchk)](https://github.com/bootchk)
* [GIMP Paint Studio](https://code.google.com/archive/p/gps-gimp-paint-studio/) został pierwotnie opracowany przez [Ramona Mirandę](https://www.ramonmiranda.com/), a obecnie [przeniesiony](https://www.deviantart.com/pkgam/art/GIMP-Paint-Studio-2-0-2-1-Port-to-GIMP-2-10-850663044) z GIMP 2.8 do 2.10+ przez [PkGam](https://www.deviantart.com/pkgam)
* [Poprawki ustawień wstępnych narzędzia GIMP 2.10](https://www.deviantart.com/pkgam/art/GIMP-2-10-Tool-Preset-Fixes-749387099) opracowane przez [PkGam](https://www.deviantart.com/pkgam)
* [SLOS-GIMPainter](https://github.com/SenlinOS/SLOS-GIMPainter) opracowane przez [SenlinOS](https://github.com/SenlinOS)
* [MyPaintBrushes-GIMP](https://github.com/SenlinOS/MyPaintBrushes-GIMP) opracowane przez [SenlinOS](https://github.com/SenlinOS)

# Licencja
Projekt jest na licencji GPL-3.0, GPL-2.0, MIT, CC BY-SA 3.0 i CC0. Więcej informacji można znaleźć w pliku LICENSE.

**- GNU General Public (GPL):**
* gps-gimp-paint-studio ([GPL-2.0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=GPL-2.0-3-ov-file))
* PhotoGIMP ([GPL-3.0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=GPL-3.0-4-ov-file))

**- Massachusetts Institute of Technology (MIT):**
* [SLOS-GIMPainter](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=MIT-5-ov-file)

**- Creative Commons (CC):**
* MyPaintBrushes-GIMP ([CC0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=CC0-1.0-1-ov-file))
* gps-gimp-paint-studio ([CC BY-SA 3.0 (Licencja na zawartość)](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=License-2-ov-file))

---

![Vimg](https://raw.githubusercontent.com/SenlinOS/databox/master/video-demo-img.jpg)

**Opis tekstowy:**

- W przypadku grafiki liniowej sprawdź opis tekstowy: [tutaj](https://github.com/SenlinOS/databox/blob/master/For-Line-Art_SLOS-GIMPainter.md).
- Ręcznie zapisz tymczasowe ustawienia wstępne, tekst + wideo: [tutaj](https://github.com/SenlinOS/databox/blob/master/manually-save-temporary-presets.md).

**Inne wskazówki:**

- Oprogramowanie GNU/Linux(X11) staje się kalką, wideo: [tutaj](https://youtu.be/ArHPMmIMsq8).

- Jak tworzyć linie perspektywiczne w programie GIMP, wideo: [tutaj](https://youtu.be/gIp5I0fXdlM).

## Współpracownicy (PhotoGIMP)
<a align="center" href="https://github.com/Diolinux/PhotoGIMP/graphs/contributors">
<img src="https://contrib.rocks/image?repo=Diolinux/PhotoGIMP" />
</a>

## Informacje o poprawce
- [Zobacz Notatki dotyczące wersji w języku portugalskim](https://diolinux.com.br/2020/06/photogimp-2020.html)
