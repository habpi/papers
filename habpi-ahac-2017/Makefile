targets=habpi-ahac-2017.pdf habpi-ahac-2017-slides.pdf 
all:$(targets) published-papers
habpi-ahac-2017.pdf: habpi-ahac-2017.tex citations.bib
	pdflatex habpi-ahac-2017.tex
	bibtex habpi-ahac-2017
	pdflatex habpi-ahac-2017.tex
	pdflatex habpi-ahac-2017.tex
habpi-ahac-2017-slides.pdf: habpi-ahac-2017-slides.tex citations.bib
	pdflatex habpi-ahac-2017-slides.tex
	bibtex habpi-ahac-2017-slides
	pdflatex habpi-ahac-2017-slides.tex
	pdflatex habpi-ahac-2017-slides.tex
published-papers: $(targets)
	cp $(targets) ../.
