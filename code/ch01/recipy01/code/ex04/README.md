Prevent a definition in a makefile from overriding the environment 
by specifying the `-e` (or `--environment-overrides`) option on the
command line of GNU make. 

```
$ export FOO=foo
$ make -e
FOO value = foo
FOO status = environment override

$ make --environment-overrides
FOO value = foo
FOO status = environment override
$ unset FOO
```