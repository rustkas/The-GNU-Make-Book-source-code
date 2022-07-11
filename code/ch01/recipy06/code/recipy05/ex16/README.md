# Delayed Variable Assignment

# Using =
```
$ make -s
Before use SHALIST is: $(eval SHALIST := $(shell find . -name '*.c' | xargs shasum))$(SHALIST)
SHALIST is: 620bf921b7bbbbf36190bc12609730ca30662f17 *./foo.c
After use SHALIST is: 620bf921b7bbbbf36190bc12609730ca30662f17 *./foo.c


```