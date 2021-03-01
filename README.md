# ThiefMD

<img src="docs/images/thiefmd_64.png" width="48" style="float: left; width: 48px" />

ThiefMD is a [Markdown](https://en.wikipedia.org/wiki/Markdown) editor that helps with `organization and management`. It is heavily inspired by [Ulysses](https://ulysses.app). Initial code was based on work from [Quilter](https://github.com/lainsce/quilter).

## Installation from Flatpak

[ThiefMD](https://flathub.org/apps/details/com.github.kmwallio.thiefmd) is now available on Flathub. Make sure you've added [flathub](https://flatpak.org/setup) to your system.

```bash
flatpak install flathub com.github.kmwallio.thiefmd
```

## Debian Based Distro Installation

```bash
sudo add-apt-repository ppa:thiefmd/thiefmd
sudo apt-get update
sudo apt-get install com.github.kmwallio.thiefmd
```

## Arch User Repository

[ThiefMD is in the Arch User Repository](https://aur.archlinux.org/packages/thiefmd) thanks to [Mark Wagie](https://github.com/yochananmarqos). You can follow [these instructions](https://wiki.archlinux.org/index.php/Arch_User_Repository#Installing_and_upgrading_packages), use [yay](https://github.com/Jguer/yay), or use your favorite AUR helper.

```bash
yay -S thiefmd
```

## Features

 * Basic library at the moment
 * Switch between documents
 * Hide Library and Document Switcher
 * Live Preview
 * Sheet Management
 * Shortcut key bindings
 * Themes
 * Export (DocX, ePUB, PDF, HTML, Markdown, [WriteFreely](https://thiefmd.com/tips/blogging-with-writefreely), [Ghost](https://thiefmd.com/tips/blogging-with-ghost), and more...)
 * Import (DocX, ePUB, HTML, rst, textile, and more...)
 * Search `Ctrl+F` for the current file, and `Ctrl+Shift+F` for the *entire* library
 * Writing Statistics
 * Focus Mode (Word, Sentence, and Paragraph)

# Translating

[Poeditor](https://poeditor.com/join/project?hash=iQkE5oTIOV) can be used to help translate ThiefMD.

 * French Translation by [David Bosman](https://github.com/davidbosman)
 * Slovak Translation by [Marek L'ach](https://github.com/marek-lach)

## Planning

 * Better library organization
 * Dedicated Markdown Editor

## Resources

 * [https://themes.thiefmd.com](https://themes.thiefmd.com) - [GitHub Source](https://github.com/ThiefMD/themes): Themes made for ThiefMD
 * [Theme-Generator](https://github.com/ThiefMD/theme-generator): GUI Application to assist in customizing ThiefMD Themes
 * [alices-adventures-in-wonderland sample novel](https://github.com/ThiefMD/sample-novel): Example project structure for writing a novel
 * [Pandoc](https://pandoc.org): Universal document converter, used for import and export. [Useful documentation on front-matter in manual](https://pandoc.org/MANUAL.html#epub-metadata)
 * [@thiefmd1 on twitter](https://twitter.com/thiefmd1): Release announcements, teasing new features, programming humor, and retweeting writing tips

## Screenshots

![](docs/images/theme_preferences.png)

Download themes from [https://themes.thiefmd.com](https://themes.thiefmd.com) or [make your own](https://themes.thiefmd.com/howto). [Ulysses Themes](https://styles.ulysses.app/themes) can also be imported through the preferences `Ctrl+,`.

![](docs/images/drag_n_drop_sheets.gif)

Drag and Drop organizing of the library.

![](docs/images/epub-export.png)

Live Preview & Export Preview

![](docs/images/typewriter_scrolling.gif)

Typewriter Scrolling.

![](docs/images/focus_mode.png)

Focus Mode

![](docs/images/write-good.png)

[Write-Good](https://github.com/ThiefMD/libwritegood-vala) recommendations and highlighting.

## Dependencies

[libwritegood-vala](https://github.com/ThiefMD/libwritegood-vala), [writeas-vala](https://github.com/ThiefMD/writeas-vala), [ghost-vala](https://github.com/ThiefMD/ghost-vala) and the [Ulysses Theme Parser](https://github.com/TwiRp/ultheme-vala) are used as git sub-modules.

### Ubuntu

```
meson
ninja-build
valac
cmake
libgtkspell3-3-dev
libwebkit2gtk-4.0-dev
libmarkdown2-dev
libxml2-dev
libclutter-1.0-dev
libarchive-dev
libgtk-3-dev
libgee-0.8-dev
libgtksourceview-4-dev
libsecret-1-dev
libhandy-1-dev
```

### Fedora

```
vala
meson
ninja-build
cmake
libmarkdown-devel
clutter-gtk-devel
webkit2gtk3-devel
gtk3-devel
gtksourceview4-devel
gtkspell3-devel
libarchive-devel
libxml2-devel
libgee-devel
libsecret-devel
libhandy1-devel
```

## Building

```bash
$ git clone https://github.com/kmwallio/ThiefMD.git
$ cd ThiefMD
$ git submodule init
$ git submodule update --remote --recursive
$ meson build && cd build
$ meson configure -Dprefix=/usr
$ ninja
$ sudo ninja install
```

[Prebuilt packages](https://github.com/kmwallio/ThiefMD/releases) are available.

## Acknowledgments

* [Contributors who help make ThiefMD awesome](https://github.com/kmwallio/ThiefMD/graphs/contributors)
* Code ~~stolen~~ *forked* from [Quilter](https://github.com/lainsce/quilter)
* Fonts are [iA Writer Duospace](https://github.com/iaolo/iA-Fonts) and [Courier Prime](https://quoteunquoteapps.com/courierprime)
* Inspired by [Ulysses](https://ulysses.app)
* Preview CSS is [Splendor](http://markdowncss.github.io/splendor) + [Modest](http://markdowncss.github.io/modest)
* Preview Scroll stolen from [this Stackoverflow](https://stackoverflow.com/questions/8922107/javascript-scrollintoview-middle-alignment) by [Rohan Orton](https://stackoverflow.com/users/2800005/rohan-orton)
* Preview Syntax Highlighting by [highlight.js](https://highlightjs.org)
* Math Rendering by [Katex](https://katex.org)
* Multi-format Export & Import by [Pandoc](https://pandoc.org)
* Write-Good based on [btford/write-good](https://github.com/btford/write-good)
