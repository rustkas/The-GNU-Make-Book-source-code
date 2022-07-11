# What’s New in GNU make 4.0

## The --trace Command Line Option


```
$ make --trace
Makefile:21: target 'part-three' does not exist
echo Make part-three
Make part-three
Makefile:15: update target 'part-one' due to: part-three
echo Make part-one
Make part-one
Makefile:18: target 'part-two' does not exist
echo Make part-two
Make part-two

```
