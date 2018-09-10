FIGURES = $(wildcard *.svg)
PDFS    = $(patsubst %.svg,%.pdf,$(FIGURES))
EPSS    = $(patsubst %.svg,%.eps,$(FIGURES))

all: $(PDFS) $(EPSS)

%.pdf: %.svg
	inkscape $< --export-pdf=$@ -D

%.eps: %.svg
	inkscape $< --export-eps=$@ -D

clean:
	rm -rf $(PDFS)
