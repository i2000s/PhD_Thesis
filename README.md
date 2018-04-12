# README

This is a template customized by Xiaodong Qi based on the UNM thesis/dissertation template.

If Maketool has been installed, go to the "main" directory, running `make all && make clean` should compile the LaTeX into a PDF file and then clean up the useless temporary files.

## Major improvements over the previous UNM PhDThesis templates

The previous template can be found [here](http://www.math.unm.edu/~gthesis/latex/).
This new template is based on the OGS LaTeX template dated on Oct 15, 2014, as well as some internal templates that have been passed along in CQuIC (by Zhang Jiang, Ben Baragiola, et al.).
Some major improvements over those previous templates are

+ Improved ease of compiling chapters independently.
+ Add necessary default sections (References, Index, etc.) and pagelinks to the Table of Content. Hyperlinks have been beautified to avoid the default ugly and distracting colors.
+ Use the latest `imakeidx` package for modern Indexing.
+ Add the latest UNM logo (Dec 2017) to the frontpage. 
+ Load necessary packages for math and physics symbols that are fully compatible with [revtex4-1 style](https://journals.aps.org/revtex). Update an example page of the List of Symbols for preview. 
+ Customizable signature page to be fully compatible with LaTeX editing and the OGS page numbering guideline. 
+ Examples of defining macro commands for interactive editing with collaborators (usually PhD supervisor) and easy cleanup tricks. There are also other macro command examples and instructions of customizations in the `styles/qxd.sty` file. 
+ Improved compatibility with `TikZ` and `PGFPlots` packages.
+ Update supported PDF version up to the stable version 1.7 (ISO 32000-1:2008). 

## Known issues and future works

+ The bottom margin of a page may be shorter than the [official requirement](http://grad.unm.edu/degree-completion/thesis-dissertations/guidelines.html) (1 inch). This might have something to do with the position of page numbers. Since many approved dissertations have been using the same bottom margin setting as this template, I didn't put much effort to verify the actual margins. 
+ I believe [PDF 2.0 (ISO 32000-2:2017)](https://www.iso.org/standard/63534.html) haven't been implemented in [PDFLaTeX](http://ctan.math.illinois.edu/systems/doc/pdftex/manual/pdftex-a.pdf) yet. Keep an eye open if metadata or other features will be needed for future updates.