ROOTNAME = ech-interop-report
PDFFILE = $(ROOTNAME).pdf
DVIFILE = $(ROOTNAME).dvi
TEXFILE = $(ROOTNAME).tex
LATEX = pdflatex
L2R = latex2rtf

all: base 

base:
	$(LATEX) $(ROOTNAME)
	bibtex $(ROOTNAME)
	$(LATEX) $(ROOTNAME)
	$(LATEX) $(ROOTNAME)

publish:
	cp ech-interop-report.pdf ..

clean:
	rm -f *.dvi *.ps *.aux *.bbl *.blg *.log *.out
