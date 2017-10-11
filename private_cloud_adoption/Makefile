ASCIIDOC=asciidoctor
HTML=$(patsubst %.adoc,%.html,$(shell find . -name \*.adoc))

all: $(HTML)

%.html: %.adoc
	cd $(<D) && $(ASCIIDOC) $(<F)

clean:
	rm -f $(HTML)

.PHONY: all clean
