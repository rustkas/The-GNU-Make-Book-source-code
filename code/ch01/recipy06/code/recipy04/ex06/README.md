# Undefined Variables in Conditionals
VAR is empty 

```
VAR =
ifdef VAR
$(info VAR is defined)
else
$(info VAR is undefined)
endif
```

Use `--warn-undefined-variables` command line option when used value is undefined.

`make --warn-undefined-variables`