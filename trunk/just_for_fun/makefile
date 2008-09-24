PAGE := 1

all: just_for_fun.pdf
just_for_fun.pdf:
	xelatex just_for_fun.tex && xelatex just_for_fun.tex

#xpdf is used for testing. You can comment that.
xpdf: just_for_fun.pdf
	xpdf $< -z width -g 1200x800 ${PAGE}

clean:
	rm -f *.log *.aux *.toc *.out *~
purge: clean
	rm -f just_for_fun.pdf