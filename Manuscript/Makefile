MS := Total_magnetization_estimation
DIFF := $(MS)_diff
REVISED := $(MS)_revised
TEX := $(MS).tex
DIFFTEX := $(DIFF).tex
REVISEDTEX := $(REVISED).tex
PDF := $(MS).pdf
DIFFPDF := $(DIFF),pdf
REVISEDPDF := $(REVISED),pdf
BIB := bib-file.bib

all: ms diff revised

ms: $(PDF)

diff: $(DIFFPDF)

revised: $(REVISEDPDF)

$(PDF): $(TEX)
	pdflatex $<
	bibtex $(MS)
	pdflatex $<
	pdflatex $<

$(DIFFPDF): $(DIFFTEX)
	pdflatex $<
	bibtex $(DIFF)
	pdflatex $<
	pdflatex $<

$(REVISEDPDF): $(REVISEDTEX)
	pdflatex $<
	bibtex $(REVISED)
	pdflatex $<
	pdflatex $<

clean:
	rm -rf *.out *.aux *.log *.bbl *.fls \
		*.blg *.fff *.lof *.lot *.ttt
