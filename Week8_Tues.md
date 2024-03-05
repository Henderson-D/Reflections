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
