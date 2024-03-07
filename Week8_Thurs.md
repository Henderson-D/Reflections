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

* && Works other way around
  * When the value to the left is false, it returns that value. Otherwise, it returns the value on its right

* The operator on the right is only evaluated when necessary.

* _true_ || X - X is NEVER be evaluated
* _false_ && X - X is NEVER evaluated
  > This was the most helpful piece of information that made this fully 'click' for me. I was fairly certain that this was the case, but visualizing a representation was very helpful

* __conditional operator__ - For second and third value, only the one that is selected is evaluated.

* ?: pick one of two values based on a third value
  * AI example was:
```
var age = 20;
var isAdult = (age >= 18) ? 'Yes' : 'No';
console.log(isAdult); // Output: 'Yes'
```
> In this example, if age is greater than or equal to 18, the condition (age >= 18) evaluates to true, so the expression 'Yes' after the ? is returned. Otherwise, the expression 'No' after the : is returned.
>
> "Shorthand, simple if-else statements" - This makes sense to me with this exact explanation.

> A few of these concepts, ?: and the functionality of || and &&, were slightly shaky; however, I believe that after looking up a few examples of each has provided me with enough information
> to have a good solid understanding of every concept mentioned. I wish that this chapter provided more examples through code blocks, as this is what makes sense to me more than an intext
> pseudocode example. Still a good read, nonetheless!
