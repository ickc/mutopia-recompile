LY = $(wildcard *.ly)
PDF = $(patsubst %.ly,%.pdf,$(LY))

pdf: $(PDF)

%.pdf: %.ly
	lilypond $<

clean:
	rm -rf $(PDF)

upgrade:
	convert-ly -e $(LY)
	find . -name '*.ly~' -delete
