.PHONY: all
.DEFAULT_GOAL = all

X=$(YS) hate $(ZS)
Y=dog
YS=$(Y)$(S)
Z=cat
ZS=$(Z)$(S)
S=s

#print-%: ; @echo $* = $($*)
print-%: ; @echo $* = $($*) from $(origin $*)

all: ; $(info X = $(X))