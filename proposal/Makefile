.PHONY : all latex bibtex pdf view clean distclean

TARGET=research-plan
SOURCE=$(TARGET).tex

all:
	@echo "Compiling at `date +'%H-%M-%S'`"
	xelatex $(SOURCE)
	bibtex $(TARGET)
	xelatex $(SOURCE)
	xelatex $(SOURCE)

latex:
	xelatex $(SOURCE)
	xelatex $(SOURCE)

bibtex:
	bibtex $(TARGET)

view:
	open $(TARGET).pdf &

clean:
	rm -f $(TARGET).aux $(TARGET).bbl $(TARGET).blg $(TARGET).log $(TARGET).out

distclean:clean
	rm -f $(TARGET).pdf
