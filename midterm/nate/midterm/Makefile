NAME	= midterm
TEXJUNK	= aux blg bbl log pdf

all: $(NAME).tex $(patsubst %,%.bib,$(BIBS))
	pdflatex $(NAME)
	bibtex   $(NAME)
	pdflatex $(NAME)
	pdflatex $(NAME)

clean:
	$(RM) $(patsubst %,$(NAME).%,$(TEXJUNK))
