# Command Detection

## Check for the existence of curly only if the download target will actually be used
```
$ make -s -k
Do all...

$ make -s -k download
which: no curly in (/mingw64/bin:/usr/local/bin:/usr/bin:/bin:/e/Windows/System32:/e/Windows:/e/Windows/System32/Wbem:/e/Windows/System32/WindowsPowerShell/v1.0/:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl)
Makefile:6: *** 'curly' missing and needed for this build.  Stop.


```