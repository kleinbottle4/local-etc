pdf_cmd = groff -Kiso-10646/utf8 -e -t -ms -s -Tpdf main.ms > main.pdf
ps_cmd  = groff -Kiso-10646/utf8 -e -t -ms -s       main.ms > main.ps
pdfv = zathura
psv = atril

main.ps: main.ms
	$(ps_cmd)

pdf : main.ms
	$(pdf_cmd)

view: main.ms
	$(psv) main.ps

loop:
	echo main.ms | entr -s "$(ps_cmd)"


