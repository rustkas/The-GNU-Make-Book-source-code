# Getting Environment Variables into GNU make

## Override variable priority list (from higher to lower)

1. `override` directive,
2. command line,
3. environment overrides (the `-e` option),
4. variables defined in a `Makefile`,
5. original environment.