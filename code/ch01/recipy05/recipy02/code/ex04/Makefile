.PHONY: all

lib1_SRCS := $(wildcard lib1/*.c)
lib2_SRCS := $(wildcard lib2/*.c)

# .c will be replaced by .o
lib1_OBJS := $(lib1_SRCS:.c=.o)
lib2_OBJS := $(lib2_SRCS:.c=.o)

.PHONY: all

all: $(lib1_OBJS) $(lib2_OBJS)
	%.o: %.c ; @$(COMPILE.C) -o $@ $<	