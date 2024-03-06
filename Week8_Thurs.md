## _Eloquent JavaScript_ Reading ##
__Empty Values__
* null
* undefined
  * Carry no information
  * _mostly_ interchangeable
> My initial thought concerning the difference between 'null' and 'undefined' was that there was at least _some_ difference. It is interesting that they are mostly interchangeable

__Automatic Type Conversion__
> This is actually one of my favorite aspects of JS so far. It is somewhat nice that you do not need to go through "double.Parse(xyz);" as you would in C#. I can definitely see this being an issue in terms of coming back to a program
> and determining what the intended input actually is.

* (x*null) will always return 0
  
```
console.log("5" - 1)
// 4
```
> This is interesting, especially because ("5" + 1) acts exactly how I would expect it to, returning 51, while the above does not act how I would initially expect.

* __Type Coercion__
  * JS converts the "wrong" type of value to the value it needs, returns unexpected values often
  * "+" will result in attempting string concatenation before numerical addition
  * When a value is not able to be obviously reassigned, it results in NaN, Not a Number

* __null == undefined__
  * returns true
  * only returns true in the case that null or undefined is being compared to null or undefined
  * to test if a value has a real value instead of null or undefined, compare it to null with == or !=

__Avoiding Automatic Type Conversion__
* use === - tests if a value is _exactly_ alike the compared value
* use !== - tests if a value is not precisely equal
* use three character comparison operators to "validate" data types. If you are sure of the data types, there is no need

__Short-circuiting of logical operators__
* && and || convert the value on the left side to a boolean in order to decide what to do
### || Characteristics ###
  * If unable to, it will return the right-side value
    
```
console.log(null || "user")
// → user
console.log("Agnes" || "user")
// → Agnes
```
> My understanding is that since null is not a value that holds information, it cannot be used to make a decision. So, it moves to "user," which holds information and can be used to make a decision.
> Since "Agnes" is an information-holding value and is on the left, it is able to be used; therefore, leaving "user" unused in this case.

* 0, NaN, "" - return false
* All other values count as true

