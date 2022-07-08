Care about is whether the variable got its value from the environment.

```
$ export VAR=ok
$ make
VAR value = ok
VAR status = environment
make: *** No targets.  Stop.

# Uncomment variable VAR definition inside Makefile and save it

$ make -e
VAR value = ok
VAR status = environment
make: *** No targets.  Stop.
$ unset VAR
```