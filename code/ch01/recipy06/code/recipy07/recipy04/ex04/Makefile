# https://www.gnu.org/software/make/manual/html_node/Text-Functions.html
# Using built-in function strip
# $(strip string)
# Using built-in function wordlist
# $(wordlist s,e,text)
# Using built-in function words
# $(words text)
# Using built-in function firstword
# $(firstword names…)
# function reduce(FUNCTION, LIST)
reduce = $(if $(strip $2), $(call reduce,$1,$(wordlist 2,$(words $2),$2), $(call strip,$(call $1,$(firstword $2),$3))),$3)

# Using built-in function filter
# $(filter pattern…,text)
# function check_uniq(LIST)
check_uniq = $(info check_uniq ($1) ($2))$(if $(filter $1,$2),$2,$2 $1)

# function uniq(LIST)
uniq = $(call strip,$(call reduce,sort,$1))

$(info c b a a c c b a c b a)
$(info $(call uniq,c b a a c c b a c b a))

.PHONY: all
.DEFAULT: all
all: ; 

