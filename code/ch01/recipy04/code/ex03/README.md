Verify environment of $(shell)

```
$ make
FOO=bar
FOO=bar

$ export FOO=foo; make; unset FOO
FOO=bar
FOO=bar

```