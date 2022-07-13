C := 1234567890 ABCDEFGHIJKLMNOPQRSTUVWXYZ
C += $C
C += $C
C += $C
C += $C
C += $C
C += $C
C += $C
C += $C
C += $C
C += $C
C += $C

FOO := $(subst 9,NINE,$C)$(subst 8,EIGHT,$C)$(subst 7,SEVEN,$C) \
$(subst 6,SIX,$C)$(subst 5,FIVE,$C)$(subst 4,FOUR,$C) \
$(subst 3,THREE,$C)$(subst 2,TWO,$C)$(subst 1,ONE,$C)
_DUMMY := $(FOO)

.PHONY: all

all: ; @echo $(_DUMMY)