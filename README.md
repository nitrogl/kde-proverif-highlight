# Syntax Highlighting for ProVerif files for KDE editors

Syntax highlight support for the applied pi-calculus language of ProVerif in KDE editors.

## Screenshot

![An extract of the Needham-Schroeder protocol - code taken from the manual.](https://raw.githubusercontent.com/nitrogl/kde-proverif-highlight/main/ns-example.jpg)

## Language support

This highlighter follows the syntax parsed by ProVerif 2.04 and the subset from CryptoVerif that is currently compatible/understood by ProVerif.

Additionally, one can use the Objective Caml doc in the comments (that start with `(**`).

## Instructions

### General instructions

To use the syntax highlighting, place the file `proverif.xml` to 

For local user       `$HOME/.local/share/org.kde.syntax-highlighting/syntax/`

For Flatpak packages `$HOME/.var/app/package-name/data/org.kde.syntax-highlighting/syntax/`

For Snap packages    `$HOME/snap/package-name/current/.local/share/org.kde.syntax-highlighting/syntax/`

On Windows&reg;      `&amp;#37;USERPROFILE&#37;&#92;AppData&#92;Local&#92;org.kde.syntax-highlighting&#92;syntax&#92;`

On macOS&reg;        `$HOME/Library/Application Support/org.kde.syntax-highlighting/syntax/`

### Linux, no cloning

It might be easier to just download a copy of the file `proverif.xml` to your local directory without cloning the whole repositor.
If you have `wget` installed in your system, you can easily do

    mkdir -p ~/.local/share/org.kde.syntax-highlighting/syntax/
    cd ~/.local/share/org.kde.syntax-highlighting/syntax/
    wget https://raw.githubusercontent.com/nitrogl/kde-proverif-highlight/main/proverif.xml

You may need to restart your editors.
If you open a `.pv` file it should automatically load the correct highlighting.

