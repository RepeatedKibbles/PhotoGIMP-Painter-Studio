OBSERVAÇÃO: Embora o projeto seja muito funcional como está e você provavelmente possa usá-lo com poucos ou nenhum problema, é importante notar que [eu](https://github.com/Diolinux) não consigo implementar novos recursos ou analisar relatórios de bugs por enquanto.
Fora isso, aproveite o PhotoGIMP Painter Studio! :)

# 🎨 PhotoGIMP Painter Studio

<img src="./.local/share/icons/hicolor/256x256/apps/photogimp.png" align="right" alt="Ícone do aplicativo PhotoGimp" title="Ícone do aplicativo PhotoGimp">

Um patch para otimizar o GIMP 2.10+ para usuários do Adobe Photoshop, incluindo recursos como:

* Organização de ferramentas para imitar a posição do Adobe Photoshop;
* Novos filtros Python instalados por padrão, como "curar seleção";
* Nova tela inicial
* Novas configurações padrão para maximizar o espaço na tela;
* Atalhos semelhantes aos do Photoshop para Windows, seguindo a documentação da Adobe;
* Novo ícone e nome do arquivo .desktop personalizado.
* O idioma do sistema agora é usado por padrão, você ainda pode alterar nas configurações se quiser.
* Os pincéis são exibidos como ícones. (Adequado para usuários de diferentes idiomas)
* Arranjo ordenado e classificação clara.
* Escolha um pincel adequado e substitua o formato do pincel para obter um novo efeito. (Evite sempre criar novos pincéis)
* Arquivos SVG (caminhos) incluídos no projeto podem ser usados ​​com pincéis para criar linhas de efeito.

![PhotoGimp Diolinux Splash Art](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/photogimp-diolinux-splash.png)
![GPS Techno Dark Splash Art](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/GPS-2_0--splash-techno-dark.jpg)

# O que é o GIMP Paint Studio (GPS)?

O GPS é uma coleção de pincéis e predefinições de ferramentas que os acompanham. As predefinições de ferramentas são opções de ferramentas salvas de forma simples, um recurso altamente útil do GIMP.

O objetivo do GPS é fornecer um ambiente de trabalho adequado para designers gráficos e artistas começarem a pintar e se sentirem confortáveis ​​com o GIMP desde o primeiro uso. Mais tarde, o usuário alterará essas configurações com base em suas próprias preferências de fluxo de trabalho e compreensão do GIMP.

Você pode aprender mais sobre GPS no [WIki](https://code.google.com/archive/p/gps-gimp-paint-studio/)

Obrigado por usá-lo! Boa pintura!
[Ramón Miranda, proprietário do GPS](www.ramonmiranda.com)

# Nome do projeto
O nome do projeto = `My Name Abbreviation` + `GIMP` + `Painter`

- A palavra `Painter` para explicar melhor a função do projeto. O GIMP é adjacente ao `P` no Painter, então os dois `P` são mesclados.

O nome do projeto é **SLOS-GIMPainter**

# MyPaintBrushes-GIMP
MyPaint-Brushes para GIMP 2.10.x

![img](https://raw.githubusercontent.com/SenlinOS/databox/master/MyPaint-Brushes-for-GIMP-2.10-By_SenlinOS.jpg)

**[I](https://github.com/SenlinOS) fiz esses MyPaint-Brushes para GIMP**.

**Estes pincéis não são adequados para MyPaint**, como “002 Frame Line” no MyPaint causará o fenômeno de “vazamento de caneta”.
<br />No GIMP 2.10, mantenha pressionada a tecla Shift “002 Frame Line” para desenhar uma linha reta.

Outros pincéis também foram depurados, como “005 Calligraph” é uma borda dura.
<br />“006 Paint Brush” para desenhar com pressão máxima, as bordas não ficarão irregulares.

**O MyPaint não precisa desses pincéis**, ele foi projetado apenas para o GIMP 2.10.
<br />E [eu](https://github.com/SenlinOS) acidentalmente excluí o arquivo “.conf” do MyPaint-brushes ao depurar…

# Estilo:
Arranjo ordenado e classificação clara.

## 📷 Capturas de tela

![Captura de tela do PhotoGimp OSX](./screenshots/osx.png)

## ⚙ Como instalar (usando Flatpak)

Este pacote é sobre flatpak, mas também contém "apenas arquivos" que você pode usar em qualquer versão do GIMP (.deb, .rpm, Snap, AppImage, Windows, macOS). Basta verificar a localização dos arquivos de configuração do GIMP.

**Inicie e feche o GIMP após a instalação antes de continuar!**

### Prepare o ambiente Flatpak

*Se você já instalou o GIMP via .deb, .rpm, etc., certifique-se de excluir o diretório `$HOME/.config/GIMP`, pois isso pode causar conflitos com os arquivos de configuração do Flatpak.*

1. Primeiro de tudo, você precisa ter o GIMP mais recente instalado no seu sistema [usando o Flatpak](https://flatpak.org/setup/)
2. Instale o GIMP Flatpak pelo AppCenter/Gerenciador de Pacotes ou terminal:
```flatpak install flathub org.gimp.GIMP```

### Instale o PhotoGIMP Painter Studio

Dentro do arquivo .zip do [PhotoGIMP-Painter-Studio-master.zip](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/archive/refs/heads/master.zip) você encontrará três pastas (ocultas em sistemas não Windows, pois seus nomes começam com um ponto). Todas essas pastas precisam ser extraídas para sua pasta `$HOME`, sobrescrevendo tudo se você já tiver os mesmos arquivos de uma instalação mais antiga.

O arquivo contém estes diretórios:

* `.icons` (que tem um novo ícone do PhotoGIMP)
* `.local` (que contém o arquivo .desktop personalizado)
* `.var` (que contém a personalização do patch flatpak para o GIMP 2.10+)

Se você quiser apenas a personalização do PhotoGIMP sem alterar o ícone original do GIMP e seu nome, basta extrair apenas a pasta ```.var``` para seu diretório inicial.

- Editar -> Preferências ->(Pastas -> MyPaint Brushes).
- Clique no botão [Adicionar uma nova pasta] para abrir o diretório [SLOS_MPB].
- Reinicie o GIMP.

## ⚙ Como instalar (outros)

Como são apenas arquivos, a única coisa que você precisa fazer é copiar todos os arquivos que residem em uma pasta específica deste pacote `/.var/app/org.gimp.GIMP/config/GIMP/2.10` para a pasta de configuração do seu GIMP em cada sistema específico, substituindo os existentes.

**Inicie e saia do GIMP após a instalação antes de continuar!**

O novo ícone precisa ser definido manualmente.

### Ubuntu Snap

Pasta de configuração: `$HOME/snap/gimp/47/.config/GIMP/2.10/`

### Outros sistemas Linux ou Unix (.deb, .rpm, etc.)

Pasta de configuração: `$HOME/.config/GIMP/2.10/`

### macOS

Pasta de configuração: `"$HOME/Library/Application Support/GIMP/2.10/"`

* [Tutorial em vídeo por Davies Media Design no macOS](https://youtu.be/5nXhtaGQs9U)

### Mac OS Easy Installer (feito por: [@MatthijsKamstra](https://github.com/MatthijsKamstra))

> O Gimp precisa ser instalado ([brew](https://formulae.brew.sh/cask/gimp) ou [caso contrário](https://www.gimp.org/downloads/))

##### Execute o bash como

você pode [down](https://raw.githubusercontent.com/MatthijsKamstra/Mac-setup/master/install/photogimp_osx.sh) e executar o script bash:

```bash
cd /caminho/para/pasta/de/download
sh photogimp_osx.sh
```

### Windows

* Baixe o arquivo [PhotoGIMP-Painter-Studio-master.zip](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/archive/refs/heads/master.zip)
* Acesse o caminho `.var\app\org.gimp.GIMP\config\GIMP\2.10` do ZIP, copie os arquivos para o caminho `%APPDATA%\GIMP\2.10`
* [Tutorial em vídeo por Davies Media Design no Windows](https://youtu.be/57DNUsf4A-0)

# Mostrar caixa de diálogo
Abra o menu Janela: Caixas de diálogo encaixáveis ​​-> Predefinições de ferramentas, e você verá o SLOS-GIMPainter.

- Clique no pequeno botão triangular no canto superior direito da caixa de diálogo Predefinições de ferramentas e clique em `Exibir como grade`.
- Clique no pequeno botão triangular no canto superior direito da caixa de diálogo Predefinições de ferramentas para `Visualizar tamanho` e selecione `Grande`.
- Selecione a aba `SLOS` no topo da caixa de diálogo Predefinições de ferramentas para ocultar as predefinições integradas.

**Após a configuração, no menu, Editar -> Preferências -> Interface (Gerenciamento de janelas), salve as configurações conforme mostrado na captura de tela e clique em OK para finalizar.**

![(Gerenciamento de janelas](https://raw.githubusercontent.com/SenlinOS/databox/master/SLOS-GIMPainter-Installation/wmment.jpg)

## Créditos

* Este projeto não seria possível sem a incrível equipe do GIMP.
* A foto no novo Splash é de [Isabella Mariana](https://www.pexels.com/pt-br/@isabella-mariana-1022505)
* Um GRANDE agradecimento a todos os apoiadores do Diolinux no [Twitch](https://twitch.tv/Diolinux) e no [YouTube](https://youtube.com/Diolinux).
* [Plugin GIMP Resynthesizer Suite](https://www.logarithmic.net/pfh/resynthesizer) foi originalmente desenvolvido por [Paul Harrison](https://logarithmic.net/pfh/) e agora assumido [manutenção](https://github.com/bootchk/resynthesizer) por [Lloyd Konneker (também conhecido como bootchk)](https://github.com/bootchk)
* [GIMP Paint Studio](https://code.google.com/archive/p/gps-gimp-paint-studio/) foi originalmente desenvolvido por [Ramon Miranda](https://www.ramonmiranda.com/) e agora [portado](https://www.deviantart.com/pkgam/art/GIMP-Paint-Studio-2-0-2-1-Port-to-GIMP-2-10-850663044) do GIMP 2.8 para 2.10+ por [PkGam](https://www.deviantart.com/pkgam)
* [Correções de predefinições de ferramentas do GIMP 2.10](https://www.deviantart.com/pkgam/art/GIMP-2-10-Tool-Preset-Fixes-749387099) desenvolvido por [PkGam](https://www.deviantart.com/pkgam)
* [SLOS-GIMPainter](https://github.com/SenlinOS/SLOS-GIMPainter) desenvolvido por [SenlinOS](https://github.com/SenlinOS)
* [MyPaintBrushes-GIMP](https://github.com/SenlinOS/MyPaintBrushes-GIMP) desenvolvido por [SenlinOS](https://github.com/SenlinOS)

# Licença
O projeto está sob uma GPL-3.0, Licença GPL-2.0, MIT, CC BY-SA 3.0 e CC0. Veja o arquivo LICENSE para mais informações.

**- GNU General Public (GPL):**
* gps-gimp-paint-studio ([GPL-2.0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=GPL-2.0-3-ov-file))
* PhotoGIMP ([GPL-3.0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=GPL-3.0-4-ov-file))

**- Instituto de Tecnologia de Massachusetts (MIT):**
* [SLOS-GIMPainter](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=MIT-5-ov-file)

**- Creative Commons (CC):**
* MyPaintBrushes-GIMP ([CC0](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=CC0-1.0-1-ov-file))
* gps-gimp-paint-studio ([CC BY-SA 3.0 (Licença para Conteúdo)](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/tree/master?tab=License-2-ov-file))

---

![Vimg](https://raw.githubusercontent.com/SenlinOS/databox/master/video-demo-img.jpg)

**Descrição do texto:**

- Para Line Art, verifique a descrição do texto: [Aqui](https://github.com/SenlinOS/databox/blob/master/For-Line-Art_SLOS-GIMPainter.md).
- Salve manualmente as predefinições temporárias, o texto+vídeo: [Aqui](https://github.com/SenlinOS/databox/blob/master/manually-save-temporary-presets.md).

**Outras dicas:**

- O software GNU/Linux(X11) se torna papel vegetal, vídeo: [Aqui](https://youtu.be/ArHPMmIMsq8).

- Como fazer linhas de perspectiva no GIMP, vídeo: [Aqui](https://youtu.be/gIp5I0fXdlM).

## Contribuidores (PhotoGIMP)
<a align="center" href="https://github.com/Diolinux/PhotoGIMP/graphs/contributors">
<img src="https://contrib.rocks/image?repo=Diolinux/PhotoGIMP" />
</a>

## Notas do Patch
- [Veja as Notas de Lançamento em Português](https://diolinux.com.br/2020/06/photogimp-2020.html)
