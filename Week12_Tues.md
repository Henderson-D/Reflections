## Pass By Copy/Value ##
* Primitive data types are pass by copy
* Objects and literal arrays are pass by reference

* After assigning a value to the primitive data type variable, that variable has nothing to do with the value that was passed to the variable. Any references made to the variable will have nothing to do with the string/number that was initially passed

* Pass by value is the same thing, just often references functions

* Since primitive data types are immutable, we are throwing out the initial value, incrementing the initial value, and that incremented value is now in its place

## Pass by reference ##
* Objects ARE mutable
  * Anything in JS that is not a primitive value
* Directly taking the reference and assigning it to newVariable
* x = 123
* y = x;
* The value, 123, is being referenced by x AND y. y does not reference x, it is essentially using x to point back to the reference value, 123.
 * Same principle for lists, arrays, primitives


