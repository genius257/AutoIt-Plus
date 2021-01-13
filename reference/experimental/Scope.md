Currently in AutoIt3

```
Global $i = 0

Func test1()
  $i = 1
EndFunc

Func test2()
  Local $i
  $i = 2
EndFunc

Func test3()
  Global $i
  $i = 3
EndFunc

test1(); $i = 1
test2(); $i = 1
test3(); $i = 3
```

In AutoIt3 the global $i would become 0, then 1 then 3

A "better" solution is to assume local scope unless global scope has been specified like so:

```
Global $i = 0

Func test1()
  $i = 1
EndFunc

Func test2()
  Local $i
  $i = 2
EndFunc

Func test3()
  Global $i
  $i = 3
EndFunc

test1(); $i = 0
test2(); $i = 0
test3(); $i = 3
```
