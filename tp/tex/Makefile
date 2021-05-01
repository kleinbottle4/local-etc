main.pdf: main.tex
	pdftex main

ps: main.tex
	tex main
	dvips main

view: main.pdf
	xdg-open main.pdf

loop:
	echo main.tex | entr -s "make &"

.PHONY:
	ps view loop
