LATEX	= pdflatex
BIBTEX	= bibtex

TITLE	= proposal
TEXJUNK	= aux log out pdf bbl blg

.PHONY: all clean

all: $(TITLE).pdf

$(TITLE).pdf: $(TITLE).tex bibliography.bib
	$(LATEX)  $(TITLE)
	$(BIBTEX) $(TITLE)
	$(LATEX)  $(TITLE)
	$(LATEX)  $(TITLE)

clean:
	$(RM) $(patsubst %,$(TITLE).%,$(TEXJUNK))
