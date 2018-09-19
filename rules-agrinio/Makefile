SRCS = $(wildcard *.tex)
MAINFILES = $(patsubst %.tex,%,$(SRCS))

.PHONY: all
all: $(MAINFILES)

%: %.tex
	xelatex $<
	xelatex $<

.PHONY: clean
clean:
	-rm -f *.aux
	-rm -f *.log
	-rm -f *.toc
	-rm -f *.bbl
	-rm -f *.blg
	-rm -f *.out

.PHONY: cleanall
cleanall: clean
	-rm -f *.pdf
	-rm -f *.ps
	-rm -f *.dvi
