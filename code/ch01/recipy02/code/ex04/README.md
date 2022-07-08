Set by default to `yes` and can be overridden either 
on the command line or in the environmen.

```
$ unset BUILD_DEBUG && make
BUILD_DEBUG is yes

$ export BUILD_DEBUG=no && make
BUILD_DEBUG is no

export BUILD_DEBUG=no && make -e
BUILD_DEBUG is no

make -e BUILD_DEBUG=no
BUILD_DEBUG is no

```