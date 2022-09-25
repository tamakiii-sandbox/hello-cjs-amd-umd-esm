.PHONY: help setup install clean uninstall
.PHONY: jscat node-test node-test-only test

help:
	@cat $(firstword $(MAKEFILE_LIST))

setup:

install: \
	node_modules

jscat: | src/index.js
	npx --no jscat $|

node-test: | src/index.js
	npx --no node--test $|

node-test-only: | src/index.js
	npx --no node--test-only $|

test: | src/index.js
	npx --no test $|

node_modules:
	npm install

clean:

uninstall:
	rm -rf node_modules
