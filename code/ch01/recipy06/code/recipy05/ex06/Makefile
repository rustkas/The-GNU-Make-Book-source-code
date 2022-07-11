TRUE = true
FALSE =

nand = $(call not, $(call and,$1,$2)) 
nor = $(call not, $(call or,$1,$2))
xor = $(call and, $(call or,$1,$2), $(call not, $(call and, $1, $2)))
$(info )
$(info nand)
$(info true,   true: $(call nand, TRUE, TRUE))
$(info true,  false: $(call nand, TRUE, FALSE))
$(info false,  true: $(call nand, FALSE, TRUE))
$(info false,  true: $(call nand, FALSE, TRUE))
$(info false, false: $(call nand, FALSE, FALSE))
$(info )
$(info nor)
$(info true,   true: $(call nor, TRUE, TRUE))
$(info true,  false: $(call nor, TRUE, FALSE))
$(info false,  true: $(call nor, FALSE, TRUE))
$(info false,  true: $(call nor, FALSE, TRUE))
$(info false, false: $(call nor, FALSE, FALSE))
$(info )
$(info xor)
$(info true,   true: $(call xor, TRUE, TRUE))
$(info true,  false: $(call xor, TRUE, FALSE))
$(info false,  true: $(call xor, FALSE, TRUE))
$(info false,  true: $(call xor, FALSE, TRUE))
$(info false, false: $(call xor, FALSE, FALSE))

.PHONY: all
.DEFAULT: all
all: ;