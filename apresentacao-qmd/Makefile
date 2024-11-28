file=index

qr:
	quarto render $(file).qmd --to revealjs

qrc:
	quarto render $(file).qmd --to revealjs --cache-refresh 

qp:
	quarto preview $(file).qmd --to revealjs

qrpdf:
	quarto render $(file).qmd --to pdf

qrall:
	quarto render $(file).qmd --to pdf
	quarto render $(file).qmd --to html
	quarto render $(file).qmd --to docx

qrhtml:
	quarto render $(file).qmd --to html

qrdocx:
	quarto render $(file).qmd --to docx 

qppdf:
	quarto preview $(file).qmd --to pdf

qphtml:
	quarto preview $(file).qmd --to html

qs:
	rsync -avzhe "ssh -i ~/.chave/chave_limpa" --info=progress2 --delete ../apresentacao-qmd/ bibr@159.89.36.185:/var/www/roneyfraga.com/public_html/class/2024-enecomat/

all:
	quarto render $(file).qmd --to revealjs
	rsync -avzhe "ssh -i ~/.chave/chave_limpa" --info=progress2 --delete ../apresentacao-qmd/ bibr@159.89.36.185:/var/www/roneyfraga.com/public_html/class/2024-enecomat/


