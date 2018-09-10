FIGURES  = $(wildcard *.svg)
PDFS     = $(patsubst %.svg,%.pdf,$(FIGURES))
PDF_TEXS = $(patsubst %.svg,%.pdf_tex,$(FIGURES))

all: $(PDFS)

%.pdf %.pdf_tex: %.svg
	inkscape $< --export-pdf=$@ -D -z --export-latex

clean:
	rm -rf $(PDFS)
	rm -rf $(PDF_TEXS)
