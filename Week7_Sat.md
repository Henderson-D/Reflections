## Fix Template Repo to Include .vscode Directory ##
* Be in correct repo
* .vscode was ignored
  * This means extensions and settings were not actually committed to GitHub
#### Make sure we have .vscode, extensions.json, and settings.json, then copy and paste the contents of settings/extensions files ####
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

## Numbers, Booleans, Comparisons, const and let

TO DO:
Numbers, Booleans, Comparisons, const and let
READING *Eloquent JavaScript*
Do Notes for Homework Review
