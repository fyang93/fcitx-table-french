# How to use (ArchLinux only)

```
git clone https://github.com/fyang93/fcitx-table-french
cd fcitx-table-french
makepkg -si .
```

To adjust the vocaburary, you may need to edit `src/tables/francais.txt` and remove `src/tables/francais.mb` before re-installation.
It takes a long time (over 1h on my laptop...) for `txt2mb` to finish processing, good luck!

All credits go to @X-Wei and his fancy [project](https://github.com/X-Wei/fcitx-table-french).
