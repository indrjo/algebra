
.PHONY: clean

.RECIPEPREFIX = >

DEPENDS = $(shell find . -type f -name '*.tex')

groups.pdf: $(DEPENDS)
> @latexmk -lualatex -lualatex='lualatex --synctex=1 %O %S' groups.tex 

clean:
> latexmk -CA

