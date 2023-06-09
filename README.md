# Syntax Highlighting for ProVerif files for KDE editors

Syntax highlight support for the applied pi-calculus language of [ProVerif](https://bblanche.gitlabpages.inria.fr/proverif/) in KDE editors ([Kate](https://kate-editor.org/get-it/), [KWrite](https://apps.kde.org/en-gb/kwrite/), [Kile](https://apps.kde.org/en-gb/kile/), ...).

## Screenshot

![An extract of the Needham-Schroeder protocol - code taken from the manual.](https://raw.githubusercontent.com/nitrogl/kde-proverif-highlight/main/ns-example.jpg)

## Language support

This highlighter follows the syntax parsed by ProVerif 2.04 and the subset from CryptoVerif that is currently compatible/understood by ProVerif.

Additionally, one can use the Objective Caml doc in the comments (that start with `(**`).

It currently does not support bound names in queries.

## Instructions

### General instructions

To use the syntax highlighting, place the file `proverif.xml` to 

For local user       `$HOME/.local/share/org.kde.syntax-highlighting/syntax/`

For Flatpak packages `$HOME/.var/app/package-name/data/org.kde.syntax-highlighting/syntax/`

For Snap packages    `$HOME/snap/package-name/current/.local/share/org.kde.syntax-highlighting/syntax/`

On Windows&reg;      `%USERPROFILE%\AppData\Local\org.kde.syntax-highlighting\syntax\`

On macOS&reg;        `$HOME/Library/Application Support/org.kde.syntax-highlighting/syntax/`

### Linux, no cloning

It might be easier to just download a copy of the file `proverif.xml` to your local directory without cloning the whole repository.
If you have `wget` installed in your system, you can easily do

    mkdir -p ~/.local/share/org.kde.syntax-highlighting/syntax/
    cd ~/.local/share/org.kde.syntax-highlighting/syntax/
    wget https://raw.githubusercontent.com/nitrogl/kde-proverif-highlight/main/proverif.xml

You may need to restart your KDE editors too see the changes.
If you open a `.pv` or `.pi` file, it should automatically load the correct highlighting.

