## Methods ##

* Methods look like Functions, but are not
```
const objectLiteral = {
 name : 'John Doe',

methodName(parameter1) {
	return `${parameter1} ${this.name}.`

}
}
```
* Notice that the method is _INSIDE_ of the function
* ${this.name} is saying "Inside of the object that you are inside of, find THIS property. In this case, the property is name, noted by ".name" at the end of "this"

> Most of the items are very clear: functions, string, number, array, so forth. The main issue that I have is 

* var is global, even if created inside of a function
 * Don't do this

__The Call Stack__

* This was a little fuzzy for me, but the explanation on the review video did better explain exactly what it was referring to.
* I like to think of this like those dolls that fit inside of one another

* Validation with UI actually makes sense, every other class has required us to include validation inside of the code, it is nice to see another option/perspective

* Closure - I absolutely need some more work with this. I really don't like the example as it doesn't fully explain closure in my opinion.
 * Since we are returning 1, it is constantly there, since it is referenced. It will stay there as long as the program is running, unless it is replaced with another value(?)

> Mostly I think that I need more review with closures, if my above example isn't true. I really would like to use these more to get a better familiarization with them.

## Data Structures ##

* Array / Object literals - groups of data

* Array's do not supply our own KEYS
* Object literals we do supply our own KEYS

* EVERYTHING IN JS IS AN OBJECT ASIDE FROM PRIMITIVES

* You can do numbers.randomName = 'randomName'
 * Never really want to do this

## Duality ##
* JS will temporarily change the primitive to an object, perform the operation, return value, then revert back to primitive data type

* NULL and undefined do not have any dot properties
* .push and .pop do make perfect sense as well

__MUTABILITY__
* This does make sense to me as well. Again, I reference this almost directly to the dolls that pop out of each other, Matryoshka dolls. You are passing the original value through different means of transport and you can mutate the means of passing the value, such as i+=1, but the original value remains

* My analogies may be slightly misworded, but it does all compute internally for me

## Overall Understanding ##
> I would really enjoy better, simpler, more descriptive examples from the text. The videos of you walking through are good, but the initial confusion from the literature can often be a blockade for that new
> more understandable information to come in. I would generally say that I am not really struggling with _anything_. I would really like to have more practice with closures, but I think that I now understand
> the idea behind them.
>
> The things that didn't change for me, I mostly didn't mention as they are concepts that I do not have any questions about for the most part. I did bring up all of the new or somewhat fuzzy ideas, however.
