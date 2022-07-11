# What’s New in GNU make 4.3

## Grouped explicit targets


```
$ make --trace
Makefile:20: update target 'hellomake.o' due to: hellomake.c hellomake.h
gcc -c -o hellomake.o hellomake.c -I.
Makefile:20: update target 'hellofunc.o' due to: hellofunc.c hellomake.h
gcc -c -o hellofunc.o hellofunc.c -I.
Makefile:23: update target 'hellomake' due to: hellomake.o hellofunc.o
gcc -o hellomake hellomake.o hellofunc.o -I.

```
