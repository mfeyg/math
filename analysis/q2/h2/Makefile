NAME=h2

show: ${NAME}.pdf
	if !(lsof ${NAME}.pdf | grep zathura); then zathura ${NAME}.pdf 2>/dev/null & fi
publish: ${NAME}.tex ${NAME}.pdf
	git add ${NAME}.tex Makefile
	git commit
	git push
	scp ${NAME}.pdf lunt:Desktop
pdf: ${NAME}.pdf
${NAME}.pdf: ${NAME}.tex
	pdflatex ${NAME}.tex
