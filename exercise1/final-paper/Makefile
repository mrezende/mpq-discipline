# 
# makefile para a compilação do documento
#
# S? Jun 23 21:13:37 BRT 2007
#

BASE_NAME = tese-exemplo

LATEX     = latex
XELATEX  = xelatex
BIBTEX    = bibtex
MAKEINDEX = makeindex

pdf: $(BASE_NAME).pdf
ps: $(BASE_NAME).ps

$(BASE_NAME).pdf: $(BASE_NAME).tex 
	$(XELATEX) $<
	$(BIBTEX) $(BASE_NAME) 
	$(MAKEINDEX) $(BASE_NAME) 
	$(XELATEX) $< 
	$(XELATEX) $<
	$(XELATEX) $<

$(BASE_NAME).ps: $(BASE_NAME).tex 
	$(LATEX) $<
	$(BIBTEX) $(BASE_NAME) 
	$(MAKEINDEX) $(BASE_NAME) 
	$(LATEX) $< 
	$(LATEX) $<
	$(LATEX) $<
	
clean:
	rm -f $(BASE_NAME)*.ps $(BASE_NAME)*.dvi *.log \
	      *.aux *.blg *.toc *.brf *.ilg *.ind \
	      missfont.log $(BASE_NAME)*.bbl $(BASE_NAME)*.pdf $(BASE_NAME)*.out \
		  $(BASE_NAME)*.lof $(BASE_NAME)*.lot \
		  *.idx
