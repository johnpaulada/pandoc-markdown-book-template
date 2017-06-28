# Pandoc Book Maker Template
Template for creating epub books from markdown using `pandoc`.

[![forthebadge](http://forthebadge.com/images/badges/built-by-hipsters.svg)](http://forthebadge.com)

## Instructions

### Install Pandoc

#### Debian, Ubuntu, and derivatives
- With package: [pandoc-1.19.2.1-1-amd64.deb](https://github.com/jgm/pandoc/releases/download/1.19.2.1/pandoc-1.19.2.1-1-amd64.deb)

#### macOS
- With `brew`:
```bash
brew install pandoc
```
- With package: [pandoc-1.19.2.1-osx.pkg](https://github.com/jgm/pandoc/releases/download/1.19.2.1/pandoc-1.19.2.1-osx.pkg)

#### Windows
- With MSI: [pandoc-1.19.2.1-windows.msi](https://github.com/jgm/pandoc/releases/download/1.19.2.1/pandoc-1.19.2.1-windows.msi)

### Create Book
1. Change to this directory.
2. Replace contents of `title.txt` and `contents.markdown`.
3. Create your book with the following syntax:
```bash
pandoc -S --epub-embed-font='oswald-opensans/opensans/OpenSans-*.ttf' --epub-embed-font='oswald-opensans/oswald/Oswald-*.ttf' --epub-stylesheet='epub.css' --epub-cover-image='cover.jpg' -o book.epub title.txt contents.markdown
```
