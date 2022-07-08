Set by default to `yes` and can be overridden either 
on the command line or in the environmen.

```
$ make
BUILD_DEBUG is yes

$ make BUILD_DEBUG=no
BUILD_DEBUG is no

$ export BUILD_DEBUG=no && make
BUILD_DEBUG is no

$ make
BUILD_DEBUG is no

$ export BUILD_DEBUG=no && make BUILD_DEBUG=aardvark
BUILD_DEBUG is aardvark


```