all:warnattachment.jar warnattachment.xpi

JAR_DIR = chrome
FILES = chrome/warnattachment.jar chrome.manifest defaults/preferences/*.js *.png install.rdf

.PHONY: warnattachment.jar

warnattachment.xpi: $(FILES)
	rm -f ../$@
	zip -r ../$@ $^

warnattachment.jar:
	$(MAKE) -C $(JAR_DIR)

