*Pandoc library for documentation in formats pdf and html*

A C:/path/ directory is created in the container, which can be mapped for use with relative file paths. Pandoc will always be run from the C:/path/ directory in the container and generate pdf file in the same directory.

Note: Put a header.tex file in the same directory. 

docker run --rm --volume "C:/path/:/data" pandoc/latex:2.6 --pdf-engine=xelatex -H header.tex --highlight-style zenburn --toc -N manual_to_pdf.md -o manual.pdf
