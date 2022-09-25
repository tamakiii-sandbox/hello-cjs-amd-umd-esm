.PHONY: help setup install run clean uninstall

help:
	@cat $(firstword $(MAKEFILE_LIST))

setup:

install: \
	node_modules

run: | src/index.js
	npx --no jscat $| | node -

node_modules:
	npm install

clean:

uninstall:
	rm -rf node_modules
