PAGE := 1
INC_PATH = include
INCLUDES = $(INC_PATH)/declaration.tex \
	   $(INC_PATH)/jff_1.tex \
	   $(INC_PATH)/jff_2.tex \
	   $(INC_PATH)/jff_3.tex \
	   $(INC_PATH)/jff_4.tex \
	   $(INC_PATH)/jff_5.tex

FILE_NAME = just_for_fun
PDF_FILE = $(FILE_NAME).pdf
TEX_FILE = $(FILE_NAME).tex
TEX = xelatex

all: $(PDF_FILE)
$(PDF_FILE):$(TEX_FILE) $(INCLUDES)
	$(TEX) $(TEX_FILE) && $(TEX) $(TEX_FILE)

#xpdf is used for testing. You can comment that.
xpdf: $(PDF_FILE)
	xpdf $(PDF_FILE) -z width -g 1200x800 $(PAGE)

clean:
	rm -f *.log $(INC_PATH)/*.aux *.aux *.toc *.out *~
purge: clean
	rm -f $(PDF_FILE)
