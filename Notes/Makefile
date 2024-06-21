default: RealAnalysis.pdf

%.pdf : %.tex bib sec
#$(MAKE) --directory=pst
	pdflatex $<
	pdflatex $<
	bibtex $*
	pdflatex $<
	pdflatex $<
	pdflatex $<

clean:
#	$(MAKE) --directory=pst clean
	$(RM) *.aux *.bbl *.blg *.log *.dvi *.toc *~ 

purge:
#	$(MAKE) --directory=pst purge
	$(RM) *.aux *.bbl *.blg *.log *.dvi *.toc *~ *.pdf */*~ *~ pst/*.pdf
