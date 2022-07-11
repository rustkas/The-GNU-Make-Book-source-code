.PHONY: all
OUTPUT_OPTION=

all: gcc %.o

%.o: CFLAGS += -g
%.o: %.c
# commands to execute (built-in):
	$(COMPILE.c) $(OUTPUT_OPTION) $<