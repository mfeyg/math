NAME=h1

show: ${NAME}.pdf
	if !(lsof ${NAME}.pdf | grep zathura); then zathura ${NAME}.pdf 2>/dev/null & fi
${NAME}.pdf: ${NAME}.tex
	pdflatex ${NAME}.tex
