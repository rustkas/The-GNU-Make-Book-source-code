# Dumping Every Makefile Variable

```
$ make
file .DEFAULT_GOAL=printvars (printvars)
file MAKEFILE_LIST=Makefile (Makefile)
file MAKEFLAGS= ()
file S=s (s)
file SHELL=/bin/sh (/bin/sh)
file X=dogs hate cats ($(YS) hate $(ZS))
file Y=dog (dog)
file YS=dogs ($(Y)$(S))
file Z=cat (cat)
file ZS=cats ($(Z)$(S))

```