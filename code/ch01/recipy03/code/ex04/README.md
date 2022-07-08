Remove a variable from the environment with `unexport`.
```
$ make
FOO is

$ FOO=foo make
FOO is

$ make FOO=foo
FOO is

```