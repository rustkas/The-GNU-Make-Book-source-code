# Calling Built-in Functions

## Recursion

```
$ make -s
c b a a c c b a c b a
check_uniq (c) ()
check_uniq (b) ( c)
check_uniq (a) ( c b)
check_uniq (a) ( c b a)
check_uniq (c) ( c b a)
check_uniq (c) ( c b a)
check_uniq (b) ( c b a)
check_uniq (a) ( c b a)
check_uniq (c) ( c b a)
check_uniq (b) ( c b a)
check_uniq (a) ( c b a)
c b a


```