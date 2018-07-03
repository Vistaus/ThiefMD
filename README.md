# ThiefMD

ThiefMD is a [Markdown](https://en.wikipedia.org/wiki/Markdown) editor that helps with organization and management.  It is heavily inspired by [Ulysses](https://ulysses.app).  Initial code was based on work from [Quilter](https://github.com/lainsce/quilter).

## Font

The included for is [iA Writer Duospace](https://github.com/iaolo/iA-Fonts).  It is licensed under the [SIL Open Font License](data/font/LICENSE.md).

## Dependencies

```
valac
libgranite-dev
libgtkspell3-3-dev
libwebkit2gtk-4.0-dev
libmarkdown2-dev
libgtkspell3-3-dev
libsqlite3-dev
gtk+-3.0
gtksourceview-3.0
meson
```

## Building

```bash
$ meson build && cd build
$ meson configure -Dprefix=/usr
$ sudo ninja install
```

## Planning

 * Typewriter Scrolling
 * Sheet Management
 * Export
 * Theming

## Acknowledgements

* Code <s>stolen</s> *forked* from [Quilter](https://github.com/lainsce/quilter)
* Inspired by [Ulysses](https://ulyssesapp.com/)