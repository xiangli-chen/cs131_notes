# makefile for pdflatex

doc = doc
bib = biblio.bib

all: $(doc).pdf
        open -a Preview.app $(doc).pdf
clean:
	rm -fv *.aux *.log *.bbl *.blg *.toc *.out *.lot *.lof $(doc).pdf
$(doc).pdf: $(doc).tex $(doc).bbl
	pdflatex $(doc)
	pdflatex $(doc)
$(doc).bbl: $(doc).tex $(bib)
	pdflatex $(doc)
	bibtex $(doc)
	

