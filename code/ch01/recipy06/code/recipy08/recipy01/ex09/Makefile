MAKE_MIN_VERSION := 3.81

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

.PHONY: all
.DEFAULT_GOAL = all

$(info Hello, World!)

$(info $(lastword one two three))

REC = foo
SIM := foo
# recursive expanded
$(info REC is $(flavor REC))
# simple expanded
$(info SIM is $(flavor SIM))

# https://www.gnu.org/software/make/manual/html_node/Conditional-Functions.html
# $(or condition1[,condition2[,condition3…]
OR1 :=
OR2 :=
OR3 :=
OK := $(or $(OR1) $(OR2) $(OR3))
$(info OK=$(OK))
$(if OK,$(info "or" result is true),$(info "or" result is false))

# $(and condition1[,condition2[,condition3…]])
AND1 :=3
AND2 :=1
AND3 :=ok
OK := $(and $(AND1) $(AND2) $(AND3))
$(info OK=$(OK))
$(if OK,$(info "and" result is true),$(info "and" result is false))

# https://www.gnu.org/software/make/manual/html_node/File-Name-Functions.html
$(info Absolute path: $(abspath ./home/jgc/bar))

# $(realpath names…)
$(info  Canonical absolute name: $(realpath Makefile))


all: ; @true


