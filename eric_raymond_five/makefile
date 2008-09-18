PAGE=1

xpdf: eric_raymond.pdf
	xpdf eric_raymond.pdf -z width -g 1200x800 ${PAGE}
all: eric_raymond.tex esr_1.tex esr_2.tex esr_3.tex esr_4.tex esr_5.tex
	xelatex eric_raymond.tex && xelatex eric_raymond.tex
	xpdf eric_raymond.pdf -z width -g 1200x800 ${PAGE}

