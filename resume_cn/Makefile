.PHONY: all clean

all: resume.pdf

resume.pdf: resume.tex resume.cls zh_CN-systemfonts.sty ctexhook.sty
	xelatex -interaction=nonstopmode -halt-on-error resume.tex
	xelatex -interaction=nonstopmode -halt-on-error resume.tex

clean:
	rm -f *.log *.aux *.bbl *.blg *.synctex.gz *.out *.toc *.lof *.idx *.ilg *.ind
