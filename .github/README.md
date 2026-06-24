# `brandstyler`

`brandstyler` automatically adapts the
style of a LaTeX document to that of a specific organisation.
It is also compatible with `beamer`, able to change
the style of many beamerthemes.

# Installation
Run the following in the command line:
1. If brandstyler.ins is present:
    `pdflatex brandstyler.ins`
2. If brandstyler.ins is absent:
    `pdflatex brandstyler.dtx`

Move `.sty` and `.cls` files to a folder that TeX can find.

# Documentation
Run the following in the command line:
```
pdflatex brandstyler.dtx
makeindex -s gind.ist -o brandstyler.ind brandstyler.idx
makeindex -s gglo.ist -o brandstyler.gls brandstyler.glo
pdflatex brandstyler.dtx
```
This automatically unpacks the package, as well.

If you are looking for comments or documentation, you won't find
any in the source. These packages make use of literate programming, which means
that the documentation is given in the form of a pdf file. You can
probably find brandstyler.pdf in this folder, by running "texdoc --view brandstyler"
in the command line, or Googling
"[your distribution] how to find package documentation".
If you're using MiKTeX, open MiKTeX console, go to
"Documentation" and look for "brandstyler".

# Contributing
Contributions of custom brand styles are highly encouraged.
Please create a pull request on our GitHub repository at
https://github.com/JesseStraat/brandstyler. Make sure to follow
the following guidelines:
1. Brand style files should follow the same structure
as the ones supplied in this package.
2. The file should be implemented and documented in
`brandstyler.dtx`. Don't forget to update the list of files.
3. Come up with a sensible, unique identifier. For example,
Utrecht University was named `uu-nl` instead of `uu` to discern
it from Uppsala Universitet (which should be named
`uu-se`). For country abbreviations, make sure to follow
[ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)
standards.
4. If possible, use freely available or open source fonts.
5. Never include logos; they are protected by copyright, and
hence cannot be part of this open source project.

If you don't have the technical knowledge to make a brand
style, feel free to open an issue on GitHub requesting one. Please include
a link to an official style guide.

---

&copy; 2026- Jesse Straat

License: [LPPL1.3c](https://www.latex-project.org/lppl.txt)

[GitHub Repository](https://github.com/JesseStraat/brandstyler)


