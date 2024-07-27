Oczywiście, oto przetłumaczony plik `README.md` na język polski:

---

NOTA: Chociaż projekt jest bardzo funkcjonalny i prawdopodobnie można go używać bez większych problemów, ważne jest, aby zauważyć, że [nie jestem](https://github.com/Diolinux) w stanie wdrażać nowych funkcji ani analizować zgłoszeń błędów na chwilę obecną.
Poza tym, ciesz się PhotoGIMP Painter Studio! :)

# 🎨 PhotoGIMP Painter Studio

<img src="./.local/share/icons/hicolor/256x256/apps/photogimp.png" align="right" alt="Ikona aplikacji PhotoGimp" title="Ikona aplikacji PhotoGimp">

Łatka optymalizująca GIMP 2.10+ dla użytkowników Adobe Photoshop, zawierająca funkcje takie jak:

* Organizacja narzędzi na wzór Adobe Photoshop;
* Nowe filtry Python instalowane domyślnie, takie jak "heal selection";
* Nowy ekran powitalny;
* Nowe domyślne ustawienia maksymalizujące przestrzeń na płótnie;
* Skróty klawiaturowe podobne do tych z Photoshopa dla Windows, zgodnie z dokumentacją Adobe;
* Nowa ikona i nazwa z niestandardowego pliku .desktop;
* Domyślnie używany jest język systemu, można go jednak zmienić w ustawieniach;
* Pędzle wyświetlane jako ikony. (Odpowiednie dla użytkowników różnych języków);
* Przejrzysta organizacja i wyraźna klasyfikacja;
* Wybierz odpowiedni pędzel i zamień kształt pędzla, aby uzyskać nowy efekt. (Unikaj ciągłego tworzenia nowych pędzli);
* Pliki SVG (Ścieżki) zawarte w projekcie mogą być używane z pędzlami do tworzenia linii efektowych.

![PhotoGimp Diolinux Splash Art](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/photogimp-diolinux-splash.png)
![GPS Techno Dark Splash Art](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/GPS-2_0--splash-techno-dark.jpg)

# Czym jest GIMP Paint Studio (GPS)?

GPS to zbiór pędzli i towarzyszących im presetów narzędziowych. Presety narzędziowe to po prostu zapisane opcje narzędzi, bardzo przydatna funkcja GIMP-a.

Celem GPS jest zapewnienie odpowiedniego środowiska pracy dla grafików i artystów, aby mogli rozpocząć malowanie i czuć się komfortowo z GIMP-em od pierwszego użycia. Później użytkownik będzie zmieniał te ustawienia zgodnie ze swoimi preferencjami i zrozumieniem GIMP-a.

Więcej informacji o GPS można znaleźć na [Wiki](https://code.google.com/archive/p/gps-gimp-paint-studio/).

Dziękujemy za korzystanie z niego! Szczęśliwego malowania!
[Ramón Miranda właściciel GPS](www.ramonmiranda.com)

# Nazwa Projektu
Nazwa projektu = `Moje Skróty Imienia` + `GIMP` + `Painter`

- Słowo `Painter` lepiej wyjaśnia funkcję projektu. GIMP jest obok `P` w Painter, więc oba `P` są połączone.

Nazwa projektu to **SLOS-GIMPainter**

# MyPaintBrushes-GIMP
MyPaint-Brushes dla GIMP 2.10.x

![img](https://raw.githubusercontent.com/SenlinOS/databox/master/MyPaint-Brushes-for-GIMP-2.10-By_SenlinOS.jpg)

**[Zrobiłem](https://github.com/SenlinOS) te pędzle MyPaint dla GIMP-a**.

**Te pędzle nie są odpowiednie dla MyPaint**, na przykład "002 Frame Line" w MyPaint powoduje "wyciekanie pióra".
<br />W GIMP 2.10, przytrzymanie klawisza Shift "002 Frame Line" pozwala rysować prostą linię.

Inne pędzle zostały również dostrojone, na przykład "005 Calligraph" ma twardą krawędź.
<br />"006 Paint Brush" rysuje przy maksymalnym nacisku, a krawędzie nie są postrzępione.

**MyPaint nie potrzebuje tych pędzli**, są one zaprojektowane tylko dla GIMP 2.10.
<br />I [przypadkowo usunąłem](https://github.com/SenlinOS) plik konfiguracyjny "MyPaint-brushes .conf" podczas debugowania...

# Styl:
Przejrzysta organizacja i wyraźna klasyfikacja.

## 📷 Zrzuty Ekranu

![Zrzut ekranu PhotoGimp OSX](./screenshots/osx.png)

## ⚙ Jak zainstalować (używając Flatpak)

Ten pakiet dotyczy Flatpak, ale zawiera również "po prostu pliki", których można użyć w dowolnej wersji GIMP-a (.deb, .rpm, Snap, AppImage, Windows, macOS). Sprawdź tylko lokalizację plików konfiguracyjnych GIMP-a.

**Uruchom i zamknij GIMP-a po zainstalowaniu, zanim będziesz kontynuować!**

### Przygotowanie środowiska Flatpak

*Jeśli wcześniej miałeś zainstalowany GIMP za pomocą .deb, .rpm itp., upewnij się, że usuniesz katalog `$HOME/.config/GIMP`, ponieważ może to powodować konflikty z plikami konfiguracyjnymi Flatpak.*

1. Przede wszystkim musisz mieć najnowszy GIMP zainstalowany na swoim systemie [używając Flatpak](https://flatpak.org/setup/)
2. Zainstaluj GIMP Flatpak przez AppCenter/Menedżer pakietów lub terminal:
   ```flatpak install flathub org.gimp.GIMP```

### Instalacja PhotoGIMP Painter Studio

Wewnątrz pliku .zip z [PhotoGIMP-Painter-Studio-master.zip](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/archive/refs/heads/master.zip) znajdziesz trzy foldery (ukryte na systemach innych niż Windows, ponieważ ich nazwy zaczynają się od kropki). Wszystkie te foldery muszą zostać wyodrębnione do katalogu `$HOME`, nadpisując wszystko, jeśli masz już te same pliki z wcześniejszej instalacji.

Plik zawiera te katalogi:

* `.icons` (który ma nową ikonę PhotoGIMP)
* `.local` (który zawiera spersonalizowany plik .desktop)
* `.var` (który zawiera niestandardową łatkę dla GIMP 2.10+)

Jeśli chcesz tylko dostosowanie PhotoGIMP bez zmiany oryginalnej ikony GIMP-a i jego nazwy, wyodrębnij tylko folder `.var` do swojego katalogu domowego.

- Edycja -> Preferencje ->(Foldery -> Pędzle MyPaint).
- Kliknij przycisk [Dodaj nowy folder], aby otworzyć katalog [SLOS_MPB].
- Uruchom ponownie GIMP-a.

## ⚙ Jak zainstalować (inne)

Ponieważ to tylko pliki, jedyne, co musisz zrobić, to skopiować wszystkie pliki znajdujące się w określonym folderze z tego pakietu `/.var/app/org.gimp.GIMP/config/GIMP/2.10` do folderu konfiguracyjnego GIMP-a na każdym systemie, nadpisując istniejące pliki.

**Uruchom i zamknij GIMP-a po zainstalowaniu, zanim będziesz kontynuować!**

Nową ikonę trzeba ustawić ręcznie.

### Ubuntu Snap

Folder konfiguracyjny: `$HOME/snap/gimp/47/.config/GIMP/2.10/`

### Inne systemy Linux lub Unix(-podobne) (.deb, .rpm, itp.)

Folder konfiguracyjny: `$HOME/.config/GIMP/2.10/`

### macOS

Folder konfiguracyjny: `"$HOME/Library/Application Support/GIMP/2.10/"`

* [Samouczek wideo Davies Media Design na macOS](https://youtu.be/5nXhtaGQs9U)

### Mac OS Easy Installer (wykonany przez: [@MatthijsKamstra](https://github.com/MatthijsKamstra))

> GIMP musi być zainstalowany ([brew](https://formulae.brew.sh/cask/gimp) lub [inaczej](https://www.gimp.org/downloads/))

##### Jak uruchomić bash

możesz [pobrać](https://raw.githubusercontent.com/MatthijsKamstra/Mac-setup/master/install/photogimp_osx.sh) i uruchomić skrypt bash:
