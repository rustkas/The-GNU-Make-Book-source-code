# Tracing Variable Values

## Tracing Variable Use

Tracing the variable Y:

```
$ make TRACE=S
Makefile:15: TRACE S
Makefile:15: TRACE S
Makefile:18: TRACE S
Makefile:19: TRACE S
make[1]: TRACE S
dog dog
make[1]: TRACE S
cat cat
Makefile:16: TRACE S
Makefile:16: TRACE S
make[1]: TRACE S
dogs hate cats

```

```
$ make TRACE=S
Makefile:15: TRACE S
Makefile:15: TRACE S
Makefile:18: TRACE S
Makefile:19: TRACE S
make[1]: TRACE S
dog dog
make[1]: TRACE S
cat cat
Makefile:16: TRACE S
Makefile:16: TRACE S
make[1]: TRACE S
dogs hate cats

```