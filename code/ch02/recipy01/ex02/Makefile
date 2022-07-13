PHONY: printvars
.DEFAULT_GOAL = printvars

X=$(YS) hate $(ZS)
Y=dog
YS=$(Y)$(S)
Z=cat
ZS=$(Z)$(S)
S=s

# https://www.gnu.org/software/make/manual/html_node/Text-Functions.html
# $(filter-out pattern…,text)

#$(foreach V,$(sort $(.VARIABLES)),
#  $(if
#    $(filter-out environment% default automatic undefined override,$(origin $V)),
#    $(info $V=$($V) ($(value $V)))
#  )
#)

printvars:
	@$(foreach V,$(sort $(.VARIABLES)), \
	$(if $(filter-out environ% default automatic undefined override, \
	$(origin $V)),$(info $(origin $V) $V=$($V) ($(value $V)))))