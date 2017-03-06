.PHONY: all clean

all: deedy_resume-openfont.pdf

%.pdf: %.xtx deedy-resume-openfont.cls publications.bib
	xelatex $(*).xtx
	bibtex $(*)
	xelatex $(*).xtx
	xelatex $(*).xtx

clean:
	rm -f *.aux *.bbl *.blg *.log *.out *.pdf
