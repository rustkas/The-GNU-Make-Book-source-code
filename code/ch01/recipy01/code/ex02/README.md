If a variable FOO is defined in the environment and automatically
imported into `GNU make`, `$(origin FOO)` will have the value `environment`.

```
$ export FOO=foo
$ make
local=environment, environment=environment
$ unset FOO
```