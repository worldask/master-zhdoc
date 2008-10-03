INCLUDES = declaration.tex \
	   esr_1.tex \
	   esr_2.tex \
	   esr_3.tex \
	   esr_4.tex \
	   esr_5.tex
FILE_NAME = eric_raymond
PDF_FILE = $(FILE_NAME).pdf
TEX_FILE = $(FILE_NAME).tex
TEX = xelatex

all: $(PDF_FILE)
$(PDF_FILE):$(TEX_FILE) $(INCLUDES)
	$(TEX) $(TEX_FILE) && $(TEX) $(TEX_FILE)

# I don't think add xpdf section here is a good idea since not everyone has xpdf
# or use it as the primary pdf viewer. So the PAGE var may be useless.
#PAGE := 1
#xpdf: eric_raymond.pdf
#       xpdf eric_raymond.pdf -z width -g 1200x800 ${PAGE}

clean:
	rm -f *.log *.aux *.toc *.out *~
purge: clean
	rm -f $(PDF_FILE)
