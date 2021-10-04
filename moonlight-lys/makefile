LY = $(wildcard *.ly)
PDF = $(patsubst %.ly,%.pdf,$(LY))

pdf: $(PDF)

%.pdf: %.ly
	lilypond $< -f PDF

clean:
	rm -rf $(PDF)

upgrade:
	convert-ly -e $(LY)
	find . -name '*.ly~' -delete
