# Using built-in function foreach
# $(foreach var,list,text)
# function map(FUNCTION, LIST)
map = $(foreach a,$2,$(call $1,$a))

# Using built-in function value
# $(value variable)
# function print_variable(VAR)
print_variable = $(info $1 ($(value $1) -> $($1)) )

# function print_variables(LIST_OF_VAR)
print_variables = $(call map,print_variable,$1)

VAR1 = foo
VAR2 = $(VAR1)
VAR3 = $(VAR2) $(VAR1)
$(call print_variables,VAR1 VAR2 VAR3)

.PHONY: all
.DEFAULT: all
all: ; 

