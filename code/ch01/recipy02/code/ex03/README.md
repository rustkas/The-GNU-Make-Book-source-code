# Build Debug or Release
Note @echo place 

```
$ make
BUILD_DEBUG is yes

$ make BUILD_DEBUG=no
BUILD_DEBUG is no

$ export BUILD_DEBUG=no
$ make
BUILD_DEBUG is yes

$ make -e
BUILD_DEBUG is no

$ make -e BUILD_DEBUG=maybe
BUILD_DEBUG is maybe
```