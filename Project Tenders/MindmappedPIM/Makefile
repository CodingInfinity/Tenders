all: clean mindMappedPIM_tender.pdf finalize

mindMappedPIM_tender.pdf: fabioStandard.pdf BrentonStandard.pdf reinhardtStandard.pdf
	pdflatex mindMappedPIM_tender.tex

BrentonStandard.pdf: BrentonStandard.tex
	pdflatex BrentonStandard.tex

fabioStandard.pdf: fabioStandard.tex
	pdflatex fabioStandard.tex

reinhardtStandard.pdf: reinhardtStandard.tex
	pdflatex reinhardtStandard.tex

clean:
	rm -f *.toc *.log *.pdf *.out *.aux

finalize:
	pdflatex mindMappedPIM_tender.tex && pdflatex mindMappedPIM_tender.tex && pdflatex mindMappedPIM_tender.tex && pdflatex mindMappedPIM_tender.tex 
