# Paper Build System

# Default target
all: manuscript.pdf

# Compile with lualatex + biber
manuscript.pdf: manuscript.tex references.bib figures/*
	lualatex -interaction=nonstopmode manuscript.tex
	biber manuscript
	lualatex -interaction=nonstopmode manuscript.tex
	lualatex -interaction=nonstopmode manuscript.tex

# Quick compile (no bib, no index)
quick:
	lualatex -interaction=nonstopmode manuscript.tex

# Clean build artifacts
clean:
	rm -f *.aux *.bbl *.bcf *.blg *.fdb_latexmk *.fls *.lof *.log *.lot *.out *.run.xml *.synctex.gz *.toc *.dvi *.ps
	rm -f manuscript.pdf

# Extreme clean (also removes figures-derived artifacts)
distclean: clean
	rm -f figures/*.pdf figures/*.png

.PHONY: all quick clean distclean