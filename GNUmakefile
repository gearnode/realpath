all: build install clean

realpath: realpath.c
	gcc -Wall -o $@ $^

build: realpath

install: build
	install -m 755 ./realpath /usr/local/bin/realpath
	cp -f ./realpath.1 /usr/share/man/man1/realpath.1

clean:
	rm ./realpath

.PHONY: build install
