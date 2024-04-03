## Functions ##
<img src="https://pbs.twimg.com/media/FGSy75sXoAkpOTS.jpg" alt="Alt text" width="300"/>

> The initial quote by Donald Knuth reminded me of this image, especially because of his reference to mini stones.

> Functions are definitely important to use for a lot of reasons. From my initial viewpoint, functions are hugely important for readability as well as the ability to call the function after creating it. Thus, being able to make a single change
> in the function is a much better option than finding everywhere you called the function and making the changes one by one.

> Creating new variables in the function is also a huge increase in being able to read the function. If you are only going to use the variable in the function, enclosing it in the function would be a fantastic option when compared to
> calling all variables somewhere else in the code, nowhere near where they are called.

## Defining a function ##
> The way that I describe functions, in an almost overly simplified way, is:
>
> Functions are a variable that completes a task. Their sole purpose is to be called later, often multiple times, to complete that task with a simple line of code rather than the block of code in the function. Just as a variable has a declared
> value, the task that takes place in the function has an output, this is the function's declared value.
>
> Maybe this is just because it is an example, but the example function in the literature has (x) as a parameter; typically I would want to include a value that lets me know what that parameter _should_ be, correct? I do know that people often
> do things like:
```
l*w*h=dimension
```
> I completely understand that, as we know what l, w, and h stands for; however, I would avoid using single-letter declarations as much as possible. It is obvious why they did it in the example, as it is simple, but still.

* Parameters are arguments that must be passed through the function, in place of the original parameters. When calling the function, the parameters must be the same data type and must have the same amount of parameters. For example:
```
function example(int, string){random code}

must be called as

function example(123, xyz){random code}

and cannot be called as

function example(xyz, zyx){random code}

because there is not an int variable in the call function parameters, the parameter data types are not met.
```
* Functions without a return statement return undefined.

* Global bindings are declared outside of a function, they are accessible throughout the entire program

* Local bindings are declared within a container, such as a function. These are only accessible within the scope of their container and are not accessible throughout the entire program

* If a binding, or variable, is declared globally and locally within a function, the function uses the local variable definition rather than the global definition.

* Nested Scope is referring to blocks and functions being able to be called within each other. For example:
  ```
  const functionName function (){
    const otherFunction() {scope for this function cant leave this container. Variables declared within are not directly able to be reference outside}
  }
  ```
* This is defined as _lexical scoping_

## Functions as Values ##
* I generally do not like the explainations and analogies provided in this section as I do not think that they are very clear

  ```
  const variableName = function(){
    xyz
  }
  if (someParameter){
    variableName = function() {reassignment to initial const variableName}
  }
  ```
* This is just referring to a variable being assigned the output of a function, this function that this variable is assigned to can change, changing the output of the variable when called

## Declaration Notation ##
* Function declarations are not part of the regular top to bottom flow of control
  * Once declared, they essentially are declared at the very beginning of the scope, being able to be accessed by everything above and below the function declaration
 
## Ar=>row Functions ##
* THIS, I was just reviewing this the other day in some online research and thought this was interesting, as it seemed pretty interesting to me, I will definitely be implementing this in my code

  ```
  const variableName = (someParameter) =>{
    xyz
  }
  ```
* If there are no parameters:
  ```
  const variableName = () =>{
    xyz
  }
  ```
* This was created to write smaller functions with a smaller footprint

## The Call Stack ##
* This is where the computer stores the context of a function being called
* When a function is called, the new context is stored at the top of the stack
* Infinite loops and a call stack that has grown too large will return with a fail message

## Optional Arguments ##
* Extra arguments are ignored and missing arguments are assigned a value of undefined
```
function minus(a, b) {
  if (b === undefined) return -a;
  else return a - b;
}

console.log(minus(10));
// → -10
console.log(minus(10, 5));
// → 5
```
* The -10 value is assigned as such as the equation became (undefined - 10) where as the 5 value is due to the equation being (10 - 5)

* You can fill in the missing parameters when they are missing by entering = after the parameter:

```
function greet(name = "stranger") {
  console.log("Hello, " + name + "!");
}

greet("John");
// Output: Hello, John!

greet();
// Output: Hello, stranger!

```

> The examples given are not necessarily hard to read, but I do not understand why they do not use basic examples like the above to showcase functionality. Overcomplication is the main issue with some of the examples
> throughout. Other than that, I do enjoy reading this material

