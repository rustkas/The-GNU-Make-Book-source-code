MAKE_MIN_VERSION := 4.0

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

.PHONY: all
.DEFAULT_GOAL = all

CC=gcc
CFLAGS=-I.
DEPS = hellomake.h
OBJ = hellomake.o hellofunc.o 

all: hellomake

%.o &: %.c $(DEPS)
	@$(CC) -c -o $@ $< $(CFLAGS)

hellomake: $(OBJ)
	@$(CC) -o $@ $^ $(CFLAGS)
	
clean:
	rm -f *.exe
	rm -f *.o