A variable imported from the environment can be overridden inside
the makefile. 

```
$ export FOO=foo
$ make
local FOO = bar
environment value FOO = file
```