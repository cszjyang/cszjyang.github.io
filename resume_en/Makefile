.PHONY: all clean

all: resume.pdf

resume.pdf: resume.tex
	xelatex -interaction=nonstopmode -halt-on-error resume.tex
	xelatex -interaction=nonstopmode -halt-on-error resume.tex

clean:
	rm -f resume.aux resume.log resume.out resume.synctex.gz
