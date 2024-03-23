## Null and Undefined ##
* Undefined - abscence of any value, not value assigned
  * Very rarely do we do this
  * let x
> It makes sense to never do this, as there is no assigned value, meaning there really is no use for the variable and you really aren't able to reference the variable.

> Null is the deliberate assignment of nothing
 * let y = null
 * I could see this being used as an inventory tracker for a video game. Psuedocode such as: if inventory id !== 12345, item = null. Would this be an applicable usecase?

> Not defined - Never referenced anywhere prior in the code

> I have used NULL in SQL; it makes sense that NULL means the same thing here. NULL is deliberately assigned when there is a possibility of a value missing, from my understanding, in SQL. So, I could see how that _may_ be applied here.

## Arrays ##
> variable name is the Title of the array

```
const exampleList = ["index0", "index1", "index2", 3, "index4"]

console.log(exampleList[0]) //index0
console.log(exampleList[1]) //index1
console.log(exampleList[2]) //index2
console.log(exampleList[3]) //3
console.log(exampleList[4]) //index4
```
* exampleList would be the title of this.

* To reassign an item in the list:
```
const exampleList = ["index0", "index1", "index2", 3, "index4"]

console.log(exampleList[0]) //index0
console.log(exampleList[1]) //index1

exampleList[0] = "newIndex0"

console.log(exampleList[0]) //newIndex0
console.log(exampleList[1]) //index1
```
* We cannot change exampleList, only the data inside of it, since it is a const.
  * To add a fifth index position: exampleList[5] = "index5"

## Object Literals ##
```
const objectList = { name: "Derrick",age: 22 }

console.log(objectList.name) // Derrick
```
* Since these values can be anything, we must use quotations to declare a string.

__Bracket notation__
```
const objectList = { name: "Derrick",age: 22 }

console.log(objectList["name"]) // Derrick
```
* Like SQL, the variable "name" is a KEY to access the data assigned to "name" // Derrick

## Variable Shadowing ##
* Do NOT recycle variable name when inside of a function
* I did go back and correct my code from the assigment, I believe.

> Const does not mean constant in the sense that we can declare something as a const and assign a function do it. This function is part of the const variable and its data can change and be mutated; thus, const is not constant in this case.

> To pass a variable as a function argument, you can do the following:
 ```
const name = `Derrick`;
const age = 22;

function verifyAdulthood(myName, myAge) {
  if (myAge < 0) {
    return `Please enter a valid age!`;
  }
  if (myAge < 18) {
    return `You are not old enough to enter, ${myName}!`;
  }

  return `Welcome, ${myName}!`;
}

console.log(verifyAdulthood(name, age));
```
> This is my corrected assignment. I was aware of this concept prior; however, I had a brief lapse in memory and I immediately saw my mistake this morning when I reviewed your feedback and opened the code.
>
> We can call the variables in place of the parameters, without passing the variables through the function aside from when we call the function.

> Function scope - contained within {}. Any variables contained within cannot be accessed outside, they are simply used inside the function and are used inside of the function only. 
