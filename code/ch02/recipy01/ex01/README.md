# Printing the Value of a Makefile Variable

```
$ make -s
dogs hate cats

$ make print-X
X = dogs hate cats

$ make print-Y
Y = dog

$ make print-YS
YS = dogs

$ make print-Z
Z = cat

$ make print-ZS
ZS = cats

$ make print-S
S = s

```

```
$ make print-Y
Y = dog from file

$ make print-YS
YS = dogs from file

$ make print-YS YS=fleas
```