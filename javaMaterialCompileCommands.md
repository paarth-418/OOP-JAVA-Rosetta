# To compile the pdf:
## -shell-escape is for the minted code
pdflatex -shell-escape java.tex

# To clean up all the other files other than .pdf and .tex created
rm *.aux *.log *.out *.pyg *.toc
