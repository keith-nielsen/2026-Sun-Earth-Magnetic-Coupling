# Paper build system (Pandoc)
#
# Canonical source is manuscript.md (Markdown). Pandoc renders it to a
# submission-quality PDF and to HTML; a LaTeX target is provided for export
# into a journal-specific template once a target journal is chosen.
#
#   make          # build manuscript.pdf (via tectonic)
#   make html     # build manuscript.html (no LaTeX toolchain needed)
#   make tex      # export manuscript.tex for journal templating
#   make clean

PANDOC      ?= pandoc
SRC         := manuscript.md
BIB         := references.bib
PDF_ENGINE  ?= tectonic

COMMON_OPTS := --from gfm \
               --metadata date="$(shell date +%Y-%m-%d)" \
               -V geometry:margin=1in \
               -V linkcolor:blue \
               -V fontsize=11pt

all: manuscript.pdf

# Primary output: PDF. tectonic (XeTeX) handles the manuscript's Unicode
# (Greek, superscripts, em-dashes) without a manual TeX install.
manuscript.pdf: $(SRC) $(BIB)
	$(PANDOC) $(SRC) $(COMMON_OPTS) --pdf-engine=$(PDF_ENGINE) -o $@

# Always-available HTML build for casual readers (no LaTeX needed).
html: manuscript.html
manuscript.html: $(SRC) $(BIB)
	$(PANDOC) $(SRC) --from gfm --standalone --toc -o $@

# LaTeX export — starting point for adapting to a journal's template.
tex: manuscript.tex
manuscript.tex: $(SRC) $(BIB)
	$(PANDOC) $(SRC) $(COMMON_OPTS) --standalone -o $@

# Phase B (optional): once in-text citations are converted to Pandoc [@key]
# form, enable automatic bibliography generation in any journal's CSL style:
#   $(PANDOC) $(SRC) $(COMMON_OPTS) --citeproc --bibliography=$(BIB) \
#       --csl=<journal-style>.csl --pdf-engine=$(PDF_ENGINE) -o manuscript.pdf

clean:
	rm -f manuscript.pdf manuscript.html manuscript.tex

.PHONY: all html tex clean
