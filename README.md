***Pandoc library for documentation in formats pdf and html***

A C:/path/ directory is created in the container, which can be mapped for use with relative file paths. Pandoc will always be run from the C:/path/ directory in the container and generate pdf file in the same directory.


**docker run --rm --volume "C:/path/:/data" pandoc/latex --pdf-engine=xelatex -H header.tex --highlight-style zenburn --toc -N manual_to_pdf.md -o manual.pdf**

- "LaTeX/Source Code Listings" to configure and insert code markdown such as: bash, JSON, console, languages, etc. in a document PDF.

**docker run --rm --volume "C:/Docker/GPS_docs/:/data" pandoc/latex --listings -H listings-setup.tex --pdf-engine=xelatex --highlight-style zenburn --toc -N manual_to_pdf.md -o manual.pdf**


Note: You have to put in the same directory this files as following:
- header.tex
- listings-setup.tex 
- manual_to_pdf.md
