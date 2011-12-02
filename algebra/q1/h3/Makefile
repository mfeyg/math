NAME=h3

show: ${NAME}.pdf
	if !(lsof ${NAME}.pdf | grep zathura); then zathura ${NAME}.pdf 2>/dev/null & fi
pdf: ${NAME}.pdf
${NAME}.pdf: ${NAME}.tex
	pdflatex ${NAME}.tex
