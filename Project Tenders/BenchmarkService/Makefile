all: clean benchmark_tender.pdf finalize

benchmark_tender.pdf: andrewStandard.pdf fabioStandard.pdf BrentonStandard.pdf reinhardtStandard.pdf
	pdflatex benchmark_tender.tex

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
	pdflatex benchmark_tender.tex && pdflatex benchmark_tender.tex && pdflatex benchmark_tender.tex && pdflatex benchmark_tender.tex
