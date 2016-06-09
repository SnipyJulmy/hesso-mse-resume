TEX = pdflatex -shell-escape -file-line-error
BIB = biber
NAME = resume_pcm
TEXFILE = ${NAME}.tex
PDFFILE = ${NAME}.pdf
BCFFILE = ${NAME}.bcf

.PHONY: all clean clean_all

all : ${PDFFILE}

${PDFFILE} : ${TEXFILE}
	${TEX} ${NAME}
	#${BIB} ${NAME}
	#${TEX} ${NAME} 
	${TEX} ${NAME} 

clean : 
	@rm *.bbl || true
	@rm *.log || true
	@rm *.out || true
	@rm *.blg || true
	@rm *.toc || true
	@rm *.aux || true
	@rm *.bak || true
	@rm *.pyg || true
	@rm *.backup || true
	@rm *.lof || true
	@rm *.synctex.gz || true
	@rm *.run.xml || true
	@rm *.bcf || true
	@rm -rf _minted* || true

clean_all : clean
	@rm ${PDFFILE} || true 
