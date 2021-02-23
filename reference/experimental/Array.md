# Dynamic array sizes

Array with a dynamic size, so they COULD work like normally, if a size is defined, but if no size is offered $a[]/$a[0] then the array can be dynamically increased in size $a[] = 123

internally we allocate more, indices and increment if we run out.

This may be difficult with multi dimention arrays.
