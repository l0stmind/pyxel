# <img src="https://raw.githubusercontent.com/kitao/pyxel/master/images/pyxel_logo_152x64.png">

[ [English](https://github.com/kitao/pyxel/blob/master/README.md) | [日本語](https://github.com/kitao/pyxel/blob/master/README.ja.md) | [中文](https://github.com/kitao/pyxel/blob/master/README.cn.md) | [한국어](https://github.com/kitao/pyxel/blob/master/README.ko.md) | [Español](https://github.com/kitao/pyxel/blob/master/README.es.md) | [Português](https://github.com/kitao/pyxel/blob/master/README.pt.md) | [Français](https://github.com/kitao/pyxel/blob/master/README.fr.md) ]

**Pyxel** est un moteur de jeu retro gaming pour Python.

Grâce à ses spécifications simples inspirées des consoles de jeux rétro, telles que ses 16 couleurs d'affichage et ses 4 cannaux sonores, vous êtes libre de créer vos propres jeux "pixel art".

<a href="https://github.com/kitao/pyxel/blob/master/pyxel/examples/01_hello_pyxel.py" target="_blank">
<img src="https://raw.githubusercontent.com/kitao/pyxel/master/pyxel/examples/screenshots/01_hello_pyxel.gif" width="48%">
</a>

<a href="https://github.com/kitao/pyxel/blob/master/pyxel/examples/02_jump_game.py" target="_blank">
<img src="https://raw.githubusercontent.com/kitao/pyxel/master/pyxel/examples/screenshots/02_jump_game.gif" width="48%">
</a>

<a href="https://github.com/kitao/pyxel/blob/master/pyxel/examples/03_draw_api.py" target="_blank">
<img src="https://raw.githubusercontent.com/kitao/pyxel/master/pyxel/examples/screenshots/03_draw_api.gif" width="48%">
</a>

<a href="https://github.com/kitao/pyxel/blob/master/pyxel/examples/04_sound_api.py" target="_blank">
<img src="https://raw.githubusercontent.com/kitao/pyxel/master/pyxel/examples/screenshots/04_sound_api.gif" width="48%">
</a>

<a href="https://github.com/kitao/pyxel/blob/master/pyxel/editor/screenshots/image_tilemap_editor.gif" target="_blank">
<img src="https://raw.githubusercontent.com/kitao/pyxel/master/pyxel/editor/screenshots/image_tilemap_editor.gif" width="48%">
</a>

<a href="https://github.com/kitao/pyxel/blob/master/pyxel/editor/screenshots/sound_music_editor.gif" target="_blank">
<img src="https://raw.githubusercontent.com/kitao/pyxel/master/pyxel/editor/screenshots/sound_music_editor.gif" width="48%">
</a>

L'interface de programmation de Pyxel fait référence aux célèbres [PICO-8](https://www.lexaloffle.com/pico-8.php) et [TIC-80](https://tic.computer/).

Pyxel est open source et gratuit. Lancez vous dans la programmation retro gaming avec Pyxel!

## Caractéristiques

- Fonctionne sous Windows, Mac et Linux
- Programmation avec Python3
- Palette de 16 couleurs fixe
- Banque de 3 images de 256x256 pixels
- 8 tilemaps de taille 256x256 pixels
- 4 canaux avec 64 sons définissables
- 8 musiques qui peuvent combiner des sons aléatoires **need information**
- Gestion clavier, souris et manette de jeu
- Éditeur d'images et de sons

### Palette de couleurs

<img src="https://raw.githubusercontent.com/kitao/pyxel/master/pyxel/examples/screenshots/05_color_palette.png">
<br><br>
<img src="https://raw.githubusercontent.com/kitao/pyxel/master/images/pyxel_palette.png">

## Installation

### Windows

En premier lieu installez [Python3](https://www.python.org/) (version 3.6.9 ou supérieure).

Lorsque vous installez Python, cochez la case **add Python to PATH**, comme ci-dessous:

<img src="https://raw.githubusercontent.com/kitao/pyxel/master/images/python_installer.png">

Ensuite installez Pyxel avec 'pip' depuis une ligne de commande (CMD):

```sh
pip install -U pyxel
```

### Mac

Tout d'abord, dans l'environnement où le gestionnaire de packages [Homebrew](https://brew.sh/) est installé, installez [Python3](https://www.python.org/) (version 3.6.9 ou supérieure) et [SDL2](https://www.libsdl.org/) avec la commande suivante:

```sh
brew install python3 sdl2 sdl2_image
```

Ensuite, redémarrez le terminal et installez Pyxel avec la commande 'pip3':

```sh
pip3 install -U pyxel
```

### Linux

Install [Python3](https://www.python.org/) (version 3.6.9 or higher) and the required packages in a way appropriate for each distribution.
Installez [Python3] (https://www.python.org/) (version 3.6.9 ou supérieure) et les packages requis pour votre distribution Linux.

**Ubuntu:**

```sh
sudo apt install python3 python3-pip libsdl2-dev libsdl2-image-dev
sudo -H pip3 install -U pyxel
```

### Autre environements

Pour installer Pyxel dans un environnement autre que ceux ci-dessus (Linux 32 bits, Raspberry PI, etc.), suivez les étapes ci-dessous pour la compilation de Pyxel:

#### Installer les outils et packages nécessaires

- C++ build toolchain (doit inclure le compileur gcc et l'utilitaire make)
- libsdl2-dev et libsdl2-image-dev
- [Python3](https://www.python.org/) (version 3.6.9 or supérieure) et l'installateur de paquet 'pip'

#### Executez les commandes suivante depuis n'importe quel dossier

```sh
git clone https://github.com/kitao/pyxel.git
cd pyxel
make -C pyxel/core clean all
pip3 install .
```

### Installation des exemples

Suite à l'installation de Pyxel, les exemples de Pyxel peuvent être installés dans le répertoire courant à l'aide de la ligne de commande suivant:

```sh
install_pyxel_examples
```

Les exemples sont les suivant:

- [01_hello_pyxel.py](https://github.com/kitao/pyxel/blob/master/pyxel/examples/01_hello_pyxel.py) - application Pyxel minimale
- [02_jump_game.py](https://github.com/kitao/pyxel/blob/master/pyxel/examples/02_jump_game.py) - jeu de plateforme avec un fichier resource Pyxel
- [03_draw_api.py](https://github.com/kitao/pyxel/blob/master/pyxel/examples/03_draw_api.py) - Demonstration de l'interface graphique
- [04_sound_api.py](https://github.com/kitao/pyxel/blob/master/pyxel/examples/04_sound_api.py) - Demonstration de l'interface sonore
- [05_color_palette.py](https://github.com/kitao/pyxel/blob/master/pyxel/examples/05_color_palette.py) - liste de la palette de couleur
- [06_click_game.py](https://github.com/kitao/pyxel/blob/master/pyxel/examples/06_click_game.py) - Un simple clicker
- [07_snake.py](https://github.com/kitao/pyxel/blob/master/pyxel/examples/07_snake.py) - Un simple Snake avec de la musique
- [08_triangle_api.py](https://github.com/kitao/pyxel/blob/master/pyxel/examples/08_triangle_api.py) - Exemple de dessin de triangles

Les exemples peuvent être executés comme n'importe quel programme Python:

**Windows:**

```sh
cd pyxel_examples
python 01_hello_pyxel.py
```

**Mac / Linux:**

```sh
cd pyxel_examples
python3 01_hello_pyxel.py
```

## Comment utiliser Pyxel?

### Créer une application Pyxel

Après avoir importé le module Pyxel dans votre code python, spécifiez d'abord la taille de la fenêtre avec la fonction `init`, La fonction `run` lancera le déroulement du programme.

```python
import pyxel

pyxel.init(160, 120)

def update():
    if pyxel.btnp(pyxel.KEY_Q):
        pyxel.quit()

def draw():
    pyxel.cls(0)
    pyxel.rect(10, 10, 20, 20, 11)

pyxel.run(update, draw)
```
Les arguments de la fonction `run` sont:
-La fonction `update` qui met à jour chaque image (frame).
-la fonction `draw` pour dessiner l'écran si nécessaire.

Dans Votre application, il est recommandé d'envelopper le code pyxel dans une classe comme ci-dessous:

```python
import pyxel

class App:
    def __init__(self):
        pyxel.init(160, 120)
        self.x = 0
        pyxel.run(self.update, self.draw)

    def update(self):
        self.x = (self.x + 1) % pyxel.width

    def draw(self):
        pyxel.cls(0)
        pyxel.rect(self.x, 0, 8, 8, 9)

App()
```
Il est aussi possible d'utiliser les fonctions `show` et `flip` pour dessiner de simple graphiques et/ou animations.

La fonction `show` affiche l'écran et attends jusqu'à ce que la touche `ESC` soit pressée.

```python
import pyxel

pyxel.init(120, 120)
pyxel.cls(1)
pyxel.circb(60, 60, 40, 7)
pyxel.show()
```

La fonction `flip` met à jour l'affichage à son execution.

```python
import pyxel

pyxel.init(120, 80)

while True:
    pyxel.cls(3)
    pyxel.rectb(pyxel.frame_count % 160 - 40, 20, 40, 40, 7)
    pyxel.flip()
```

### Commandes spéciales

Les Commandes spéciales suivantes peuvent êtres utilisées pendant l'exécution d'une application Pyxel:

- `Esc`<br>
Quitter l'application
- `Alt(Option)+1`<br>
Sauvegarder une capture d'écran sur le bureau
- `Alt(Option)+2`<br>
Initialise le point de départ d'une capture de l'écran en format GIF
- `Alt(Option)+3`<br>
Sauvegarde une capture d'écran (sur le bureau) sous format gif (jusqu'a 30 secondes)
- `Alt(Option)+0`<br>
Moniteur de performance (fps, update time, and draw time)
- `Alt(Option)+Enter`<br>
Activez/désactivez le plein écran

### Créer un fichier 'resource'

L'éditeur Pyxel permet de créer des images et des sons pouvant être utilisés dans un programme Pyxel.

Cet éditeur est accessible via la ligne de commande ci-dessous:

```sh
pyxeleditor [fichier_ressource_Pyxel]
```

Si le fichier ressource spécifié existe, il est chargé dans l'éditeur. Dans le cas contraire un fichier est créé avec le nom spécifié dans la ligne de commande.
Si aucun fichier n'est spécifié dans la ligne de commande, lorsque vous sauvegardez votre travail dans l'éditeur, un fichier nommé `my_resource.pyxres` sera créé automatiquement.  


After starting Pyxel Editor, the file can be switched by dragging and dropping another resource file. If the resource file is dragged and dropped while holding down ``Ctrl``(``Cmd``) key, only the resource type (image/tilemap/sound/music) that is currently being edited will be loaded. This operation enables to combine multiple resource file into one.

The created resource file can be loaded with the `load` function.

Pyxel Editor has the following edit modes.

**Image Editor:**

The mode to edit the image banks.

<img src="https://raw.githubusercontent.com/kitao/pyxel/master/pyxel/editor/screenshots/image_editor.gif">

By dragging and dropping a png file onto the Image Editor screen, the image can be loaded into the currently selected image bank.

**Tilemap Editor:**

The mode to edit tilemaps in which images of the image banks are arranged in a tile pattern.

<img src="https://raw.githubusercontent.com/kitao/pyxel/master/pyxel/editor/screenshots/tilemap_editor.gif">

**Sound Editor:**

The mode to edit sounds.

<img src="https://raw.githubusercontent.com/kitao/pyxel/master/pyxel/editor/screenshots/sound_editor.gif">

**Music Editor:**

The mode to edit musics in which the sounds are arranged in order of playback.

<img src="https://raw.githubusercontent.com/kitao/pyxel/master/pyxel/editor/screenshots/music_editor.gif">

### Other resource creation methods

Pyxel images and tilemaps can also be created in the following way:

- Create an image from a list of strings with `Image.set` or `Tilemap.set` function
- Load a png file in Pyxel palette with `Image.load` function

Pyxel sounds can also be created in the following way:

- Create a sound from strings with `Sound.set` or `Music.set` function

Please refer to the API reference for usage of these functions.

### How to Create a Stand-Alone Executable

By using the attached Pyxel Packager, a stand-alone executable that will work even in environments where Python is not installed can be created.

To create a stand-alone executable, specify the Python file to be used to launch the application with the `pyxelpackager` command as follows:

```sh
pyxelpackager python_file
```

When the process is complete, a stand-alone executable is created in the `dist` folder.

If resources such as .pyxres and .png files are also necessary, put them under the `assets` folder and they will be included.

It is also possible to specify an icon with the ``-i icon_file`` option.

## API Reference

### System

- `width`, `height`<br>
The width and height of the screen

- `frame_count`<br>
The number of the elapsed frames

- `init(width, height, [caption], [scale], [palette], [fps], [quit_key], [fullscreen])`<br>
Initialize the Pyxel application with screen size (`width`, `height`). The maximum width and height of the screen is 256<br>
It is also possible to specify the window title with `caption`, the display magnification with `scale`, the palette color with `palette`, the frame rate with `fps`, the key to quit the application with `quit_key`, and whether to start in full screen with `fullscreen`. `palette` is specified as a list of 16 elements of 24 bit color.<br>
e.g. `pyxel.init(160, 120, caption="Pyxel with PICO-8 palette", palette=[0x000000, 0x1D2B53, 0x7E2553, 0x008751, 0xAB5236, 0x5F574F, 0xC2C3C7, 0xFFF1E8, 0xFF004D, 0xFFA300, 0xFFEC27, 0x00E436, 0x29ADFF, 0x83769C, 0xFF77A8, 0xFFCCAA], quit_key=pyxel.KEY_NONE, fullscreen=True)`

- `run(update, draw)`<br>
Start the Pyxel application and call `update` function for frame update and `draw` function for drawing

- `quit()`<br>
Quit the Pyxel application at the end of the current frame

- `flip()`<br>
Force drawing the screen (do not use in normal applications)

- `show()`<br>
Draw the screen and wait forever (do not use in normal applications)

### Resource

- `save(filename)`<br>
Save the resource file (.pyxres) to the directory of the execution script

- `load(filename, [image], [tilemap], [sound], [music])`<br>
Read the resource file (.pyxres) from the directory of the execution script. If ``False`` is specified for the resource type (image/tilemap/sound/music), the resource will not be loaded.

### Input
- `mouse_x`, `mouse_y`<br>
The current position of the mouse cursor

- `mouse_wheel`<br>
The current value of the mouse wheel

- `btn(key)`<br>
Return `True` if `key` is pressed, otherwise return `False` ([key definition list](https://github.com/kitao/pyxel/blob/master/pyxel/__init__.py))

- `btnp(key, [hold], [period])`<br>
Return `True` if `key` is pressed at that frame, otherwise return `False`. When `hold` and `period` are specified, `True` will be returned at the `period` frame interval when the `key` is held down for more than `hold` frames

- `btnr(key)`<br>
Return `True` if `key` is released at that frame, otherwise return `False`

- `mouse(visible)`<br>
If `visible` is `True`, show the mouse cursor. If `False`, hide it. Even if the mouse cursor is not displayed, its position is updated.

### Graphics

- `image(img, [system])`<br>
Operate the image bank `img`(0-2) (see the Image class). If `system` is `True`, the image bank for system can be accessed. 3 is for the font and resource editor. 4 is for the display screen<br>
e.g. `pyxel.image(0).load(0, 0, "title.png")`

- `tilemap(tm)`<br>
Operate the tilemap `tm`(0-7) (see the Tilemap class)

- `clip(x, y, w, h)`<br>
Set the drawing area of the screen from (`x`, `y`) to width `w` and height `h`. Reset the drawing area to full screen with `clip()`

- `pal(col1, col2)`<br>
Replace color `col1` with `col2` at drawing. `pal()` to reset to the initial palette

- `cls(col)`<br>
Clear screen with color `col`

- `pget(x, y)`<br>
Get the color of the pixel at (`x`, `y`)

- `pset(x, y, col)`<br>
Draw a pixel of color `col` at (`x`, `y`)

- `line(x1, y1, x2, y2, col)`<br>
Draw a line of color `col` from (`x1`, `y1`) to (`x2`, `y2`)

- `rect(x, y, w, h, col)`<br>
Draw a rectangle of width `w`, height `h` and color `col` from (`x`, `y`)

- `rectb(x, y, w, h, col)`<br>
Draw the outline of a rectangle of width `w`, height `h` and color `col` from (`x`, `y`)

- `circ(x, y, r, col)`<br>
Draw a circle of radius `r` and color `col` at (`x`, `y`)

- `circb(x, y, r, col)`<br>
Draw the outline of a circle of radius `r` and color `col` at (`x`, `y`)

- `tri(x1, y1, x2, y2, x3, y3, col)`<br>
Draw a triangle with vertices (`x1`, `y1`), (`x2`, `y2`), (`x3`, `y3`) and color `col`

- `trib(x1, y1, x2, y2, x3, y3, col)`<br>
Draw the outline of a triangle with vertices (`x1`, `y1`), (`x2`, `y2`), (`x3`, `y3`) and color `col`

- `blt(x, y, img, u, v, w, h, [colkey])`<br>
Copy the region of size (`w`, `h`) from (`u`, `v`) of the image bank `img`(0-2) to (`x`, `y`). If negative value is set for `w` and/or `h`, it will reverse horizontally and/or vertically. If `colkey` is specified, treated as transparent color

- `bltm(x, y, tm, u, v, w, h, [colkey])`<br>
Draw the tilemap `tm`(0-7) to (`x`, `y`) according to the tile information of size (`w`, `h`) from (`u`, `v`). If `colkey` is specified, treated as transparent color. A tile of the tilemap is drawn with a size of 8x8, and if the tile number is 0, indicates the region (0, 0)-(7, 7) of the image bank, if 1, indicates (8, 0)-(15, 0)

- `text(x, y, s, col)`<br>
Draw a string `s` of color `col` at (`x`, `y`)

### Audio

- `sound(snd, [system])`<br>
Operate the sound `snd`(0-63) (see the Sound class). If `system` is `True`, the sound 64 for system can be accessed<br>
e.g. `pyxel.sound(0).speed = 60`

- `music(msc)`<br>
Operate the music `msc`(0-7) (see the Music class)

- `play_pos(ch)`<br>
Get the sound playback position of channel `ch`. The 100's and 1000's indicate the sound number and the 1's and 10's indicate the note number. When playback is stopped, return `-1`

- `play(ch, snd, loop=False)`<br>
Play the sound `snd`(0-63) on channel `ch`(0-3). Play in order when `snd` is a list

- `playm(msc, loop=False)`<br>
Play the music `msc`(0-7)

- `stop([ch])`<br>
Stop playback of all channels. If `ch`(0-3) is specified, stop the corresponding channel only

### Image Class

- `width`, `height`<br>
The width and height of the image

- `data`<br>
The data of the image (256x256 two-dimentional list)

- `get(x, y)`<br>
Retrieve the data of the image at (`x`, `y`)

- `set(x, y, data)`<br>
Set the data of the image at (`x`, `y`) by a value or a list of strings<br>
e.g. `pyxel.image(0).set(10, 10, ["1234", "5678", "9abc", "defg"])`

- `load(x, y, filename)`<br>
Read the png image from the directory of the execution script at (`x`, `y`)

- `copy(x, y, img, u, v, w, h)`<br>
Copy the region of size (`w`, `h`) from (`u`, `v`) of the image bank `img`(0-2) to (`x`, `y`)

### Tilemap Class

- `width`, `height`<br>
The width and height of the tilemap

- `data`<br>
The data of the tilemap (256x256 two-dimentional list)

- `refimg`<br>
The image bank referenced by the tilemap

- `get(x, y)`<br>
Retrieve the data of the tilemap at (`x`, `y`)

- `set(x, y, data)`<br>
Set the data of the tilemap at (`x`, `y`) by a value or a list of strings.<br>
e.g. `pyxel.tilemap(0).set(0, 0, ["000102", "202122", "a0a1a2", "b0b1b2"])`

- `copy(x, y, tm, u, v, w, h)`<br>
Copy the region of size (`w`, `h`) from (`u`, `v`) of the tilemap `tm`(0-7) to (`x`, `y`)

### Sound Class

- `note`<br>
List of note(0-127) (33 = 'A2' = 440Hz)

- `tone`<br>
List of tone(0:Triangle / 1:Square / 2:Pulse / 3:Noise)

- `volume`<br>
List of volume(0-7)

- `effect`<br>
List of effects(0:None / 1:Slide / 2:Vibrato / 3:FadeOut)

- `speed`<br>
The length of one note(120 = 1 second per tone)

- `set(note, tone, volume, effect, speed)`<br>
Set a note, tone, volume, and effect with a string. If the tone, volume, and effect length are shorter than the note, it is repeated from the beginning

- `set_note(note)`<br>
Set the note with a string made of 'CDEFGAB'+'#-'+'0123' or 'R'. Case-insensitive and whitespace is ignored<br>
e.g. `pyxel.sound(0).set_note("G2B-2D3R RF3F3F3")`

- `set_tone(tone)`<br>
Set the tone with a string made of 'TSPN'. Case-insensitive and whitespace is ignored<br>
e.g. `pyxel.sound(0).set_tone("TTSS PPPN")`

- `set_volume(volume)`<br>
Set the volume with a string made of '01234567'. Case-insensitive and whitespace is ignored<br>
e.g. `pyxel.sound(0).set_volume("7777 7531")`

- `set_effect(effect)`<br>
Set the effect with a string made of 'NSVF'. Case-insensitive and whitespace is ignored<br>
e.g. `pyxel.sound(0).set_effect("NFNF NVVS")`

### Music Class

- `ch0`<br>
List of sound(0-63) play on channel 0. If an empty list is specified, the channel is not used for playback

- `ch1`<br>
List of sound(0-63) play on channel 1. If an empty list is specified, the channel is not used for playback

- `ch2`<br>
List of sound(0-63) play on channel 2. If an empty list is specified, the channel is not used for playback

- `ch3`<br>
List of sound(0-63) play on channel 3. If an empty list is specified, the channel is not used for playback

- `set(ch0, ch1, ch2, ch3)`<br>
Set the list of sound(0-63) of all channels. If an empty list is specified, that channel is not used for playback<br>
e.g. `pyxel.music(0).set([0, 1], [2, 3], [4], [])`

- `set_ch0(data)`<br>
Set the list of sound(0-63) of channel 0

- `set_ch1(data)`<br>
Set the list of sound(0-63) of channel 1

- `set_ch2(data)`<br>
Set the list of sound(0-63) of channel 2

- `set_ch3(data)`<br>
Set the list of sound(0-63) of channel 3

## How to Contribute

### Submitting an issue

Use the [issue tracker](https://github.com/kitao/pyxel/issues) to submit bug reports and feature/enhancement requests.
Before submitting a new issue, search the issue tracker to ensure that there is no similar open issue.

When submitting a report, select the appropriate template from [this link](https://github.com/kitao/pyxel/issues/new/choose).

### Manual testing

Anyone manually testing the code and reporting bugs or suggestions for enhancements in the issue tracker are very welcome!

### Submitting a pull request

Patches/fixes are accepted in form of pull requests (PRs). Make sure the issue the pull request addresses is open in the issue tracker.

Submitted pull request is deemed to have agreed to publish under [MIT license](https://github.com/kitao/pyxel/blob/master/LICENSE).

## Other Information

- [Wiki](https://github.com/kitao/pyxel/wiki)
- [Subreddit](https://www.reddit.com/r/pyxel/)
- [Discord server (English)](https://discord.gg/FC7kUZJ)
- [Discord server (Japanese - 日本語版)](https://discord.gg/qHA5BCS)

## License

Pyxel is under [MIT license](http://en.wikipedia.org/wiki/MIT_License). It can be reused within proprietary software provided that all copies of the licensed software include a copy of the MIT License terms and the copyright notice.

Pyxel uses the following libraries:

- [SDL2](https://www.libsdl.org/)
- [miniz-cpp](https://github.com/tfussell/miniz-cpp)
- [PyInstaller](https://www.pyinstaller.org/)
