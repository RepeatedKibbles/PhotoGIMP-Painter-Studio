NOTA: Embora o projeto esteja muito funcional como está e você provavelmente possa usá-lo com poucos ou nenhum problema, é importante notar que [eu](https://github.com/Diolinux) não estou em condições de implementar novos recursos ou analisar relatórios de bugs no momento.
Fora isso, aproveite o PhotoGIMP Painter Studio! :)

# 🎨 PhotoGIMP Painter Studio

<img src="./.local/share/icons/hicolor/256x256/apps/photogimp.png" align="right" alt="Ícone do aplicativo PhotoGimp" title="Ícone do aplicativo PhotoGimp">

Um patch para otimizar o GIMP 2.10+ para usuários do Adobe Photoshop, incluindo recursos como:

* Organização de ferramentas para imitar a posição do Adobe Photoshop;
* Novos filtros Python instalados por padrão, como "seleção de cura";
* Nova Tela de Boas-vindas
* Novas configurações padrão para maximizar o espaço na tela;
* Atalhos semelhantes aos do Photoshop para Windows, seguindo a documentação da Adobe;
* Novo ícone e Nome do arquivo .desktop personalizado.
* O idioma do sistema agora é usado por padrão, você ainda pode mudar nas configurações se desejar.
* Pincéis são exibidos como Ícones. (Adequado para usuários de diferentes idiomas)
* Arranjo ordenado e classificação clara.
* Escolha um Pincel adequado e substitua a forma do pincel para obter um novo efeito. (Evite sempre criar novos pincéis)
* Arquivos SVG (Caminhos) incluídos com o projeto podem ser usados com pincéis para criar linhas de efeito.

![Foto de Boas-vindas do PhotoGimp Diolinux](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/photogimp-diolinux-splash.png)
![Foto de Boas-vindas Techno Dark do GPS](./.var/app/org.gimp.GIMP/config/GIMP/2.10/splashes/GPS-2_0--splash-techno-dark.jpg)

# O que é o GIMP Paint Studio (GPS)?

GPS é uma coleção de pincéis e predefinições de ferramentas. As predefinições de ferramentas são simplesmente opções de ferramentas salvas, um recurso altamente útil do GIMP.

O objetivo do GPS é fornecer um ambiente de trabalho adequado para designers gráficos e artistas começarem a pintar e se sentirem confortáveis com o GIMP desde o primeiro uso. Posteriormente, o usuário mudará essas configurações com base em suas próprias preferências de fluxo de trabalho e compreensão do GIMP.

Você pode aprender mais sobre o GPS na [WIki](https://code.google.com/archive/p/gps-gimp-paint-studio/)

Obrigado por usá-lo! Feliz pintura!
[Ramón Miranda proprietário do GPS](www.ramonmiranda.com)

# Nome do Projeto
O nome do projeto = `Minha Abreviação do Nome` + `GIMP` + `Painter`

- A palavra `Painter` para explicar melhor a função do projeto. GIMP está adjacente ao `P` em Painter, então os dois `P` são mesclados.

O nome do projeto é **SLOS-GIMPainter**

# MyPaintBrushes-GIMP
MyPaint-Brushes para GIMP 2.10.x

![img](https://raw.githubusercontent.com/SenlinOS/databox/master/MyPaint-Brushes-for-GIMP-2.10-By_SenlinOS.jpg)

**[Eu](https://github.com/SenlinOS) fiz esses MyPaint-Brushes para GIMP**.

**Esses pincéis não são adequados para MyPaint**, como "002 Frame Line" no MyPaint apresentará fenômeno de "vazamento de caneta".
<br />No GIMP 2.10, mantendo pressionada a tecla Shift, "002 Frame Line" pode desenhar uma linha reta.

Outros pincéis também foram depurados, como "005 Calligraph" tem uma borda dura.
<br />"006 Paint Brush" ao desenhar com pressão máxima, as bordas não ficarão irregulares.

**MyPaint não precisa desses pincéis**, eles foram projetados apenas para GIMP 2.10.
<br />E [eu](https://github.com/SenlinOS) acidentalmente excluí o arquivo "conf" dos pincéis MyPaint durante a depuração...

# Estilo:
Arranjo ordenado e classificação clara.

## 📷 Capturas de Tela

![Captura de Tela do PhotoGimp OSX](./screenshots/osx.png)

## ⚙ Como Instalar (usando Flatpak)

Este pacote é todo sobre flatpak, mas também contém "apenas arquivos" que você pode usar em qualquer versão do GIMP (.deb, .rpm, Snap, AppImage, Windows, macOS). Basta verificar a localização dos arquivos de configuração do GIMP.

**Inicie e saia do GIMP após a instalação antes de continuar!**

### Prepare o ambiente Flatpak

*Se você instalou o GIMP anteriormente via .deb, .rpm, etc., certifique-se de excluir o diretório `$HOME/.config/GIMP`, pois isso pode causar conflitos com os arquivos de configuração do Flatpak.*

1. Primeiramente, você precisa ter a última versão do GIMP instalada no seu sistema [usando Flatpak](https://flatpak.org/setup/)
2. Instale o GIMP Flatpak através do seu Centro de Aplicativos/Gerenciador de Pacotes ou terminal:
   ```flatpak install flathub org.gimp.GIMP```

### Instale o PhotoGIMP Painter Studio

Dentro do arquivo .zip do [PhotoGIMP-Painter-Studio-master.zip](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/archive/refs/heads/master.zip) você encontrará três pastas (ocultas em sistemas não-Windows, pois seus nomes começam com um ponto). Todas essas pastas devem ser extraídas para sua pasta `$HOME`, sobrescrevendo tudo se você já tiver os mesmos arquivos de uma instalação anterior.

O arquivo contém esses diretórios:

* `.icons` (que possui um novo ícone do PhotoGIMP)
* `.local` (que contém o arquivo .desktop personalizado)
* `.var` (que contém a personalização do patch flatpak para o GIMP 2.10+)

Se você quiser apenas a personalização do PhotoGIMP sem mudar o ícone original do GIMP e seu nome, basta extrair apenas a pasta ```.var``` para seu diretório pessoal.

- Editar -> Preferências -> (Pastas -> Pincéis do MyPaint).
- Clique no botão [Adicionar uma nova pasta] para abrir o diretório [SLOS_MPB].
- Reinicie o GIMP.

## ⚙ Como Instalar (outros)

Como são apenas arquivos, a única coisa que você precisa fazer é copiar todos os arquivos que estão em uma pasta específica deste pacote `/.var/app/org.gimp.GIMP/config/GIMP/2.10` para a pasta de configuração do GIMP em cada sistema específico, sobrescrevendo os existentes.

**Inicie e saia do GIMP após a instalação antes de continuar!**

O novo ícone precisa ser configurado manualmente.

### Ubuntu Snap

Pasta de configuração: `$HOME/snap/gimp/47/.config/GIMP/2.10/`

### Outros sistemas Linux ou Unix(-like) (.deb, .rpm, etc.)

Pasta de configuração: `$HOME/.config/GIMP/2.10/`

### macOS

Pasta de configuração: `"$HOME/Library/Application Support/GIMP/2.10/"`

* [Tutorial em Vídeo por Davies Media Design no macOS](https://youtu.be/5nXhtaGQs9U)

### Instalador Fácil para Mac OS (feito por: [@MatthijsKamstra](https://github.com/MatthijsKamstra))

> O Gimp precisa estar instalado ([brew](https://formulae.brew.sh/cask/gimp) ou [de outra forma](https://www.gimp.org/downloads/))

##### Executar bash como

você pode [baixar](https://raw.githubusercontent.com/MatthijsKamstra/Mac-setup/master/install/photogimp_osx.sh) e executar o script bash:

```bash
cd /path/to/download/folder
sh photogimp_osx.sh
```

### Windows

* Baixe o arquivo [PhotoGIMP-Painter-Studio-master.zip](https://github.com/RepeatedKibbles/PhotoGIMP-Painter-Studio/archive/refs/heads/master.zip)
* Acesse o caminho `.var\app\org.gimp.GIMP\config\GIMP\2.10` do ZIP, copie os arquivos para o caminho `%APPDATA%\GIMP\2.10`
* [Tutorial em Vídeo por Davies Media Design no Windows](https://youtu.be/57DNUsf4A-0)

# Mostrar Diálogo
Abra o menu Janela: Diálogos Acopláveis -> Predefinições de Ferramentas, e você pode ver o SLOS-GIMPainter.

- Clique no pequeno botão triangular no canto superior direito do diálogo de Predefinições de Ferramentas e clique em `Ver como Grade`.
- Clique no pequeno botão triangular no canto superior direito do diálogo de Predefinições de Ferramentas para `Tamanho da Pré-visualização` e selecione o `Grande`.
- Selecione a guia `SLOS` na parte superior do diálogo de Predefinições de Ferramentas para ocultar as predefinições embutidas.

	**Depois de configurar, no menu, Editar -> Preferências -> Interface (Gerenciamento de Janelas), salve
