
.PHONY: all html clean

OUT:=..

HTMLS:=index.html coding.html credits.html
OUTS:=$(patsubst %.html,$(OUT)/%.html,$(HTMLS))

all:
	@echo Usage: make html - makes the HTML output in ./out

html: $(OUTS)

../%.html: %.html
	php -c . $<  > $@

clean:
	rm -rf $(OUTS)
