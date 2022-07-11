SHALIST = $(eval SHALIST := $(shell find . -name '*.c' | xargs shasum))$(SHALIST)

$(info Before use SHALIST is: $(value SHALIST))
$(info SHALIST is: $(SHALIST))
$(info After use SHALIST is: $(value SHALIST))

.PHONY: all
.DEFAULT: all
all: ;
