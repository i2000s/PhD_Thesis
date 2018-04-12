#!Bash
# This makefile is for compiling LaTeX into pdf with bib libraries.
# On Windows, it requires Make tool and you may be able to add this tool by adding the MinGW to path:
#  PATH=$PATH:/MINGW/msys/1.0/bin
# where /MINGW is where MinGW is installed. The line ending should be LF.
PROJECT=main
LATEXFLAGS?=-interaction=nonstopmode -file-line-error -shell-escape
TEMPSUFFS=ps log aux out dvi bbl blg auxlock brf idx ilg ind lof toc lot

#pdf: ps
#	$(foreach proj,$(PROJECT),ps2pdf ${proj}.ps;)

#pdf-print: ps
#	$(foreach proj,$(PROJECT),ps2pdf -dColorConversionStrategy=/LeaveColorUnchanged -dPDFSETTINGS=/printer ${proj}.ps;)

#text: html
#	$(foreach proj,$(PROJECT),html2text -width 100 -style pretty ${proj}/${proj}.html | sed -n '/./,$$p' | head -n-2 >${proj}.txt;)

#html:
#	$(foreach proj,$(PROJECT),@#latex2html -split +0 -info "" -no_navigation ${proj}; \
#	htlatex ${proj};)

#ps:	dvi
#	$(foreach proj,$(PROJECT),dvips -t letter ${proj}.dvi;)

#dvi:
#	$(foreach proj,$(PROJECT),latex ${proj}; \
#	bibtex ${proj}||true; \
#	latex ${proj}; \
#	latex ${proj};)

.DEFAULT: all
.PHONY: all clean

all:
	$(foreach proj,$(PROJECT), pdflatex $(LATEXFLAGS) $(proj); \
	bibtex $(proj)||true; \
	pdflatex $(LATEXFLAGS) $(proj); \
	pdflatex $(LATEXFLAGS) $(proj); \
	pdflatex $(LATEXFLAGS) $(proj);)

read:
	evince $(foreach proj,$(PROJECT),${proj}.pdf ) &

aread:
	acroread $(foreach proj,$(PROJECT),${proj}.pdf )

clean:
	rm -f $(foreach proj,$(PROJECT),$(foreach suff, $(TEMPSUFFS), $(proj).${suff}))
