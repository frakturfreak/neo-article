# neo-article

## Purpose

This is the draft for an article about the [Neo keyboard layout](http://neo-layout.org/) for [Die TeXnische Komödie (DTK)](http://www.dante.de/DTK.html), written in the german language.

The main author is [Arno Trautmann](http://github.com/alt/neo-article).

## How to Compile

## Using the makefile

To compile, just execute the makefile:

    xelatex --shell-escape makefile

Insert 1 if you want to compile all files or 2 if you only want to compile the helper files (`ebene*.tex` and `neo*.tex`)

The option `--shell-escape` *is* needed here!

## By hand

If you want to compile by hand, you have to run `xelatex` on `ebene*.tex` first, afterwards the article can be compiled with `xelatex neo+xelatex.tex`. For bibliography, you must complement `bibtex neo+xelatex` and recompile the article with `xelatex neo+xelatex.tex`. (the `.bib` will be generated automatically in the first `neo+xelatex` run.)

## Other Versions (for pdfLaTeX)

The delivered version for the DTK had to use pdfLaTeX; it can be found unter the [abgabe tag](http://github.com/alt/neo-article/tree/abgabe). A slightly better version *may* be aviable in the `pdflatex` branch.