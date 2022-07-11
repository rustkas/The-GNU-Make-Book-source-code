# Replace character from one to another
# function char_replace(STRING, WHAT_REPLACE, SUBSTITUTION_CHARACTER)
char_replace = $(subst $1,$2,$3)

# Change file separetor
# function dos_to_unix(DOS_PATH)
dos_to_unix = $(call char_replace,\,/,$1)

# Change file separetor
# function unix_to_dos(UNIX_PATH)
unix_to_dos = $(call char_replace,/,\,$1)

unix_to_dos2 = $(subst /,\,$1)

.PHONY: all
.DEFAULT: all
all:
	$(info )
	$(info Input path: $(INPUT_PATH))
	$(info DOS TO UNIX: $(call dos_to_unix, $(INPUT_PATH)))
	$(info DOS TO UNIX: $(call dos_to_unix, github\code\ch01\recipy06\code\recipy07\recipy01\ex02))
	$(info UNIX TO DOS: $(call unix_to_dos, github/code/ch01/recipy06/code/recipy07/recipy01/ex01))
	$(info 2. UNIX TO DOS: $(call unix_to_dos2, github/code/ch01/recipy06/code/recipy07/recipy01/ex01))
	$(info feet on the street -> $(subst ee,EE,feet on the street))

