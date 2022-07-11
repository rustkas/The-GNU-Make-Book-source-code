# What’s New in GNU make 4.0

## Syncing Output with --output-sync


```
$ make
one line start
one line middle
one line finish
two line start
two line middle
two line finish
three line start
three line middle
three line finish
four line start
four line middle
four line finish

```

The targets will be built in parallel if you use the `-j` option.

```
$ make -j
one line start
two line start
three line start
four line start
one line middle
one line finish
two line middle
two line finish
three line middle
three line finish
four line middle
four line finish

```

Run four jobs in parallel

```
$ make -j4
one line start
two line start
three line start
four line start
one line middle
one line finish
two line middle
two line finish
three line middle
three line finish
four line middle
four line finish

```

Specifying -Otarget (or `--output-sync=target`) causes make to keep track.

```
$ make -j4 -Otarget
one line start
one line middle
one line finish
two line start
two line middle
two line finish
three line start
three line middle
three line finish
four line start
four line middle
four line finish

```

```
$ make -j4 --output-sync=target
one line start
one line middle
one line finish
two line start
two line middle
two line finish
three line start
three line middle
three line finish
four line start
four line middle
four line finish

```

`output-sync=recurse` handles recursive sub­makes

```
$ make -j4 --output-sync=recurse
one line start
one line middle
one line finish
two line start
two line middle
two line finish
three line start
three line middle
three line finish
four line start
four line middle
four line finish
```