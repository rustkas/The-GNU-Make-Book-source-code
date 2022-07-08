Guarantee that the variable gets its value inside Makefile:

```
$ export VAR=ok
$ make
VAR value = bar
VAR status = override
make: *** No targets.  Stop.


$ make -e
VAR value = bar
VAR status = override
make: *** No targets.  Stop.
```