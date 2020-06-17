*Pandoc library for documentation in formats pdf and html*

Put a header.tex file in the same folder. 

docker run --rm --volume "C:/path/:/data" pandoc/latex:2.6 --pdf-engine=xelatex -H header.tex --highlight-style zenburn --toc -N manual_to_pdf.md -o manual.pdf
