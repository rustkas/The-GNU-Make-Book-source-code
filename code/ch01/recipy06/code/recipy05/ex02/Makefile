make-truth = $(if $1,T,empty)

TRUE = true
FALSE =
or = $(call make-truth, $1$2)

$(info or)
$(info true,   true: $(call or,TRUE,TRUE))
$(info true,  false: $(call or,TRUE,FALSE))
$(info false,  true: $(call or,FALSE,TRUE))
$(info false,  true: $(call or,FALSE,TRUE))
$(info false, false: $(call or,FALSE,FALSE))