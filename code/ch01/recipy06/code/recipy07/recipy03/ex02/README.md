# Calling Built-in Functions

## map function implementation

```
$ make -s
VAR1 (foo -> foo)
VAR2 ($(VAR1) -> foo)
VAR3 ($(VAR2) $(VAR1) -> foo foo)

```