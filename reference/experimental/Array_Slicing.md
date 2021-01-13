Currently in AutoIt3, an array can only be resized from the end.

```
Dim $a = ['a','b','c']
ReDim $a[2]
; $a = ['a']
```

But with IDispatch interface, the memory of the array can be accessed, and functionality like `array_slice` or `array_shift` could be possible.
This is also possible in original AutoIt3 via a function call, but maybe a more seamless way in AutoItPlus could be implemented?
