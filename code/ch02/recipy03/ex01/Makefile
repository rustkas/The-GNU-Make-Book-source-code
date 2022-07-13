MYVAR1 = hello
MYVAR2 = $(MYVAR1) everyone

all: MYVAR3 = $(MYVAR2)
all: foo bar
	$(__BREAKPOINT)
	@echo Finally making $@
foo bar:
	@echo Building $@