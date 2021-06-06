NAME=mbic_analysis

all: mbic_analysis

.PHONY: clean

mbic_analysis:
	pdflatex $(NAME).tex
	bibtex $(NAME).aux
	pdflatex $(NAME).tex
	pdflatex $(NAME).tex

view: mbic_analysis
	evince $(NAME).pdf &

clean:
	rm *.blg *.bbl *.aux *.log *.out
