## Strings ##
"This is a string example!"  
console.log("32 This is also a string! 123")  
"12" + "34" = "1234"  

## Numbers ##
123  
123.456  
3+5 * 10 = 53  
(3+5) * 10 = 80  
__Exponents__ - 123e4  
Numbers do not have to be declared as a float, int, etc. 

## Booleans ##
ALWAYS return True OR False  
* console.log(2>3) returns False  
* console.log(3>2) returns True  
* console.log(!(3>2)) returns False
```
const temperature = 25;
const isSummer = True;

if (temperature > 30 && isSummer) {
    console.log("It's a hot summer day!");
} else {
    console.log("It's not too hot today.");
}
```
## Variables ##

__const__ - constant reference, a variable that cannot be reassigned.
```
  const variName = 123;
  variName = 1234;
```
 * TypeError: Assignment to constant variable.  
  
__let__ - TEMPORARILY assigned value, meaning it can be reassigned
```
  let variName = 123;
  console.log(variName)
```  
  * output > 123  
      
```  
  let variName = 1234;
  console.log(variName)
```  
  * output > 1234
    
## Operators ##
* Basic operators are:
  * "+" - addition
  * "-" - subtraction
  * "*" - multiplication
  * "/" - division
  * "%" -  remainder after division
    * 10 % 3 = 1
  * PEMDAS applies, typical math rules are followed
    
__Logical Operators__
* || - or
* && - and
* ! - not, the opposite of the value before ! is applied
  
## Template Literals ##
### Example that uses operators, variables, template literals, while loop, and logical operators ###
```
const currentWeather = 60;

while (currentWeather >= 60 && currentWeather <= 85){
console.log(`The temperature outside is: ${currentWeather}\u00B0F`);
currentWeather +=1;
}
```
> This is an inclusive loop that will execute from values 60 through 85

## Primitive Data Type ##
* A data type that only holds a single piece of data
 > const dogAge = 17;

## Strict Comparision ##
* = is an assignment
* == is a comparision. Does not have to be same data type to be true
* x === "x" is a strict comparision. This means the items must be exactly alike and the same data type to be true
* !== applies as a not equal to, essentially means "not ==="

## HW Review / General Notes ##
* You can reassign a variable from a numerical value to a string value without declaring the data type
* Data that we are creating is being stored in a generic area of memory called the heap.
  * We access this data by referencing it, or calling the related function

> There were a few things that were new to me, such as something simple like ===. However, there were a few concepts, like xyz = !yxz. I knew this existed, but have not used it and have forgotten about it. It is a very easy way to say,
> "If that is true, then this is false." Also, the function to include codeblock's now is very nice to know. There have been times where I like to use examples, because I do refer back to these reflections fairly often as a simple refresher.
> Actually, in the past, I had to go out of my way to circumvent my code, such as html, from being processed in these files.
>
> I have enjoyed the similarities of C#, but I am now excited that we are beginning to look into new concept to me and tie back into using JavaScript with this next assignment as well.
