default: pres.pdf

%.pdf: %.md
	pandoc $< -o $@ -t beamer -s --latex-engine xelatex --template beamer.tex

%.html: %.md
	pandoc -t dzslides -o $@ $< --self-contained
