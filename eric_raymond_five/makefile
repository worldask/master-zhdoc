all: eric_raymond.pdf
eric_raymond.pdf:
	xelatex eric_raymond.tex && xelatex eric_raymond.tex
# I don't think add xpdf section here is a good idea since not everyone has xpdf
# or use it as the primary pdf viewer. So the PAGE var may be useless.
#PAGE := 1
#xpdf: eric_raymond.pdf
#       xpdf eric_raymond.pdf -z width -g 1200x800 ${PAGE}
clean:
	rm -f *.log *.aux *.toc *.out
purge: clean
	rm -f eric_raymond.pdf
