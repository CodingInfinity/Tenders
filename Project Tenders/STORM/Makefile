all: clean storm_tender.pdf finalize

storm_tender.pdf: andrewStandard.pdf fabioStandard.pdf BrentonStandard.pdf reinhardtStandard.pdf
	pdflatex storm_tender.tex

andrewStandard.pdf: andrewStandard.tex
		pdflatex andrewStandard.tex

BrentonStandard.pdf: BrentonStandard.tex
	pdflatex BrentonStandard.tex

fabioStandard.pdf: fabioStandard.tex
	pdflatex fabioStandard.tex

reinhardtStandard.pdf: reinhardtStandard.tex
	pdflatex reinhardtStandard.tex

clean:
	rm -f *.toc *.log *.pdf *.out *.aux

finalize:
	pdflatex storm_tender.tex && pdflatex storm_tender.tex && pdflatex storm_tender.tex && pdflatex storm_tender.tex
