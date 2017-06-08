NAME	= annot-bib
TEXJUNK	= aux blg bbl log pdf

all: $(NAME).tex $(NAME).bib
	pdflatex $(NAME)
	bibtex   $(NAME)
	pdflatex $(NAME)
	pdflatex $(NAME)

clean:
	$(RM) $(patsubst %,$(NAME).%,$(TEXJUNK))
