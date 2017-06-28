# Pandoc Book Maker Template
[![forthebadge](http://forthebadge.com/images/badges/built-by-hipsters.svg)](http://forthebadge.com)

## Instructions

### Install Pandoc
#### macOS
```bash
brew install pandoc
```

### Create Book
1. Go to directory
2. Replace contents of `title.txt` and `contents.markdown`.
3. Create a book with the following syntax:
```bash
pandoc -S --epub-embed-font='oswald-opensans/opensans/OpenSans-*.ttf' --epub-embed-font='oswald-opensans/oswald/Oswald-*.ttf' --epub-stylesheet='epub.css' --epub-cover-image='cover.jpg' -o book.epub title.txt contents.markdown
```
