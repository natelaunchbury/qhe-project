LATEX	= pdflatex
TITLE	= presentation
TEXJUNK	= aux out log pdf snm toc nav
MODULES	= steven ben nate

all: $(TITLE).pdf

$(TITLE).pdf: $(TITLE).tex $(patsubst %,%.tex,$(MODULES))
	$(LATEX) $<
	$(LATEX) $<

clean:
	$(RM) $(patsubst %,$(TITLE).%,$(TEXJUNK)) $(patsubst %,%.aux,$(MODULES))
