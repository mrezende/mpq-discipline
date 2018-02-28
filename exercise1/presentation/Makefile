# LaTeX makefile for slides-exemplo-beamer
#
# by J.P.Mena-Chalco
#
# Sex Set 30 20:12:33 BRT 2011

PDFLATEX = pdflatex
BASE_NAME = slides-exemplo-beamer
BIBTEX    = bibtex

all: pdf
pdf: $(BASE_NAME).pdf

$(BASE_NAME).pdf: $(BASE_NAME).tex
	$(PDFLATEX) $<
	$(BIBTEX) $(BASE_NAME)
	$(PDFLATEX) $<
	$(PDFLATEX) $<
	$(PDFLATEX) $<

clean:
	rm -f $(BASE_NAME).ps $(BASE_NAME).dvi $(BASE_NAME).log \
	      $(BASE_NAME).aux $(BASE_NAME).blg $(BASE_NAME).toc \
	      missfont.log $(BASE_NAME).bbl $(BASE_NAME).pdf $(BASE_NAME).out \
				$(BASE_NAME).nav $(BASE_NAME).snm $(BASE_NAME).brf 
