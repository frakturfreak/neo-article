# neo-article

## Purpose

This is an article about the [Neo keyboard layout](http://neo-layout.org/) and XeLaTeX, written in the german language. It was also published in [Die TeXnische Komödie (DTK 2/2010)](http://www.dante.de/DTK.html), the journal of the german TeX User Group (DANTE).

The main author is [Arno Trautmann](http://github.com/alt/neo-article).

## How to Compile

## Using the makefile

To compile, just execute the makefile:

    xelatex --shell-escape makefile

Insert 1 if you want to compile all files or 2 if you only want to compile the helper files (`ebene*.tex` and `neo*.tex`)

The option `--shell-escape` *is needed* here!

## By hand

If you want to compile by hand, you have to run `xelatex` on `ebene*.tex` first, afterwards the article can be compiled with `xelatex neo+xelatex.tex`. For bibliography, you must complement `bibtex neo+xelatex` and recompile the article with `xelatex neo+xelatex.tex`. (the `.bib` will be generated automatically in the first `neo+xelatex` run.)

## Other Versions (for pdfLaTeX)

The actual delivered version for the DTK had to use pdfLaTeX; it can be found unter the [abgabe tag](http://github.com/alt/neo-article/tree/abgabe). A slightly better version *may* be aviable in the `pdflatex` branch.