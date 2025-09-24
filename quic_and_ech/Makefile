ROOTNAME = quic-and-ech
PDFFILE = $(ROOTNAME).pdf
DVIFILE = $(ROOTNAME).dvi
TEXFILE = $(ROOTNAME).tex
LATEX = pdflatex
L2H = latex2html

all: base 

publish:
	cp ech-interop-report.pdf ..

base:
	$(LATEX) $(ROOTNAME)
	bibtex $(ROOTNAME)
	$(LATEX) $(ROOTNAME)
	$(LATEX) $(ROOTNAME)

html:
	$(L2H) $(ROOTNAME)
	bibtex $(ROOTNAME)
	$(L2H) $(ROOTNAME)
	$(L2H) $(ROOTNAME)

clean:
	rm -f *.dvi *.ps *.aux *.bbl *.blg *.log *.out html/
