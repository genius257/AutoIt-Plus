AutoIt3 has For In, but this gives little control key => value wise.

A Foreach solution is needed

```
  $aArray = StringSplit("abcd", "", 2)
  
  Foreach $aArray in $key, $value
    ConsoleWriteLine($key)
    ConsoleWriteLine($value)
  Next
```

should give:

```
0
a
1
b
2
c
3
d
```
