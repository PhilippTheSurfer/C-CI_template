.PHONY: build install clean

build: personal_helpers.c personal_helpers.h
	gcc -c personal_helpers.c -o personal_helpers.o
	ar -rc libpersonal_helpers.a personal_helpers.o

install: build
	cp libpersonal_helpers.a /usr/local/lib
	cp personal_helpers.h /usr/local/include

clean:
	rm personal_helpers.o
	rm libpersonal_helpers.a
