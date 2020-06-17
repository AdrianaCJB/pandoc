# pandoc
Run a pandoc docker for documentation with format pdf and html.

Put a header.tex file in the same folder. 

docker run --rm --volume "C:/<path>/:/data" pandoc/latex:2.6 --pdf-engine=xelatex -H header.tex --highlight-style zenburn --toc -N README.md -o README.pdf
