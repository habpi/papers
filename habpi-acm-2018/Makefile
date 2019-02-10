targets=habpi-acm-2018.pdf
all:$(targets) published-papers
habpi-acm-2018.pdf: habpi-acm-2018.tex citations.bib
	pdflatex habpi-acm-2018.tex
	pdflatex habpi-acm-2018.tex
	bibtex habpi-acm-2018
	pdflatex habpi-acm-2018.tex
	pdflatex habpi-acm-2018.tex
	pdflatex habpi-acm-2018.tex
published-papers: $(targets)
	cp $(targets) ../.
clean:
	rm `cat .gitignore`
