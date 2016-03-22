TARGETS = $(shell ls *tex | sed 's/tex$$/pdf/g')

all: ${TARGETS}

%.pdf: %.tex
	xelatex $<

tidy:
	rm -f *.{aux,log}

clean: tidy
	rm -f ${TARGETS}
