.PHONY: all

all: foo.o bar

bar: ; @touch $@

CC := gcc
%.o : %.c
	@@$(CC) -o $@ $^