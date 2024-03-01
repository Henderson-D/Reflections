## Fix Template Repo to Include .vscode Directory ##
* Be in correct repo
* .vscode was ignored
  * This means extensions and settings were not actually committed to GitHub
    
#### Make sure we have .vscode, extensions.json, and settings.json, then copy and paste the contents of settings/extensions files ####
> Completed on 2/27 at 6:24pm

* In real code, you mostly don't want to overuse console statements
* Semi-colon - automatically inserted if they are not present, are optional but corrected by eslint or prettier formatting
* Semi-colon is like a period, an end of a thought. Not fully needed, but it is proper to use them. USE THEM
##### CANNOT USE LINE BREAKS WHEN DOING RETURN #####
* Block of code - group of code contained within {}
##### CONST #####
* = is an assignment operator, functions from right to left
  * const 1[sum] = 2[addNumbers(5,10)];
  * grabs information to be used[2] then assigns it to declared variable[1]
  * Kind of like how SQL uses FROM before SELECT
* const [name] = [data you want to store in memory]

> Interesting that you can do "sum = xyz;" and exclude const. I agree, this would be a terrible error and relatively unreadable in the future. What does JavaScript define sum as in this case as far as data type,
> when it is not declared by us? Does it default to const?

## Re-Read the *Eloquent JavaScript* Example Codes ##
* let - similar to const
  * const is used to create a variable, just like let
  * CONST DOES NOT MEAN CONSTANT
    * I did assume that it meant constant as in a non-changing variable
    * It does seem my idea of const was correct, I believe
* let - line of code is TEMPORARILY assigned to the VARIABLE
  * exemplified by +=

* let [create variable];  
  while (condition statement)  
  {loop to execute while condition statement is true)  
  output
* += takes initial value, removes it, then places new value in its place

> let total = 0, count = 1;  
> while (count <=10){  
> total += count;  
> count += 1;  
> }  
> console. log (total);

> [declare variables]  
> [set condition statement]  
> [total reassigned to initial value + [count] value (total=total+count)]  
> [count value equals itself + 1, x=x+1]  
> [output]

* While STOPS looping when the condition statement is FALSE

## READING *Eloquent JavaScript* ##

## Strings ##
* Strings, Numbers, and Booleans can all be assigned as a CONST
* Strings can be used with:
  * ""
  * ''
  * ``
  * MUST BE STARTED AND ENDED WITH SAME TYPE
  * USE `` when doing template literals ${XYZ}
  * > I found this to be interesting, considering JS has been defined as relaxed up to this point
* To change variable name in all use-cases, use F2
* Template literal is better than concatenation in this example (and probably most cases)

## Numbers, Booleans, Comparisons, const and let ##

**Numerical Values**
* There is no declaration of int, float, double, etc.
* You just create a numerical value and JS figures it out
  
**Booleans**
* Either True or False
* const isGreater = age > 18
  * This will be true as long as age is greater than 18
  * Used to compare values/variables
  * Can be used to do loops
* Named after George Bool
    
**Const isn't reassignable, let is**  
*let variableName = 123;  
variableName = 321

## What does const actually mean? ##
* a constant reference to a specified value
* const variables cannot be reassigned

## Primitive Data Types ##
* often simple and are known as discrete data
* One individual piece of data
* Cannot be changed or mutated
* Must use let if we want to modify the value of a variable
  * dating(let) VS marriage(const)

# Reading *Eloquent JavaScript* #
* _"Inside the computer’s world, there is only data. "_
  > This is essentially true for our physical world too. While there are events that seem non-data-related, they are data-driven and derived. War is a game of logistics, which is driven by data.
  > Without data, war is lost. Without data, there cannot be rational decision-making. Without data, there is chaos; chaos stems from senseless actions, like a syntax error.

* Bits are 0 and 1
  * 0 - Low electrical charge
  * 1 - High electrical charge

* Increase from right to left
  * 128, 64, 32, 16, 8, 4, 2, 1
    > This is an interesting way to look at it. Another class goes over this as well, but it was not explained this simple, for whatever reason.

> Is a bit a fixed size?
 > I do not think that it is, considering that the evolution of products would be severely limited. However, I would assume that the storage of each bit would be limited, at some point.
 > In the case that we reach whatever theoretical shrinking constraint there is, it would be interesting to see if we traverse the path of shrinking programs. As wrong as it sounds, a 
 > theoretical instance in which a bit exists that is neither on nor off would likely be a solution.
 >
 > I think this would be like UTF-8 compared to UTF-16. There are 8 missing data areas, which are non-existent in UTF-8. However, you could look at this as if the 8 missing digits were neither   > positively or negatively charged. Probably all mumbo-jumbo, but an interesting concept.

* Separate data into chunks to represent pieces of information, called _values_ in JS

* To call a value, you just invoke its name
  > I completely understand the necessity of using values for the sake of time, legibility, and countless other reasons; however as devil's advocate, when you call the value, would it cause       > some very small delay as opposed to typing the data the value holds? For example, instead of having 2+3 directly in front of you, you would have to determine that xyz = 123 and then assign    > 123 in its place. Again, simply just talking about the most basic, unnoticed delays being possible.

* JS uses 64 bits to store a single number value

* The value of different numbers is actually _limited_
  > This is interesting, yet unsurprising.

*  Maximum whole number that can be stored is around 9 quadrillion(15 zeros)

* fractions are with a decimal
* very large or small with e (for exponent)

* Math functions exactly how you would expect

* % is the remainder property, like C#

__SPECIAL NUMBERS__
* Infinity
* -Infinity
* NaN - Not a Number

__Strings__
* Function like normal, use '',"",``
* \n - New Line
* Unicode standard used but uses 16 bits per string element
* emoji's take us two character positions
* Strings cannot be divided, multiplied, or subtracted __THEY ARE CONCATENATED__

__Unary Operators__
> console.log(typeof 1.5)  
> // → number
* Not entirely sure that I understand the typeof operator. My understanding is that it will return whether the value is a type of string or number. However, what exact benefit would this give you?

* binary operator - takes two values
* unary operator - takes one value

__Boolean__
* True or False
* Used for cases like "Yes or No" and "On or Off"
__Comparison__
> console.log(3 > 2)  
> // → true
* Used to produce a boolean Value

> console.log("Aardvark" < "Zoroaster")  
> // → true
* You can compare strings, Uppercase letters are less than lowercase. More characters will be greater as well

* There is only one value in JavaScript that is not equal to itself, and that is NaN (“not a number”).
> console.log(NaN == NaN)  
> // → false

> This makes sense, as you cannot compare a non-number that is also a non-string

__Logical Operators__
* AND - &&
* OR - ||
* NOT - !
* Pretty much just like C# in terms of how it works

__Comparison Operators__
* >, <, <=, =>, etc

__Ternary Operator__
> console.log(true ? 1 : 2);  
> // → 1  
> console.log(false ? 1 : 2);  
> // → 2

* Conditional operator
* When true, it picks the middle value
* When false, it chooses value on the right
