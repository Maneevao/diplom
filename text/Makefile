all: textcopy.pdf
	mv textcopy.pdf result.pdf
	rm textcopy.*
textcopy.pdf: textcopy.tex
	xelatex textcopy.tex
	bibtexu textcopy
	xelatex textcopy.tex
	xelatex textcopy.tex
textcopy.tex:
	cp text.tex textcopy.tex
clean:
	rm -rf textcopy.* result.pdf *.log
