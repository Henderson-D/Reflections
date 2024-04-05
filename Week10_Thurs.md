## Code Differences ##
> When reviewing my code, it appears that there are two differences, both related. Where I use people[i].name and people[i].age, you use person.name and person.age after assigning person to people[i]
>
> Effectively our code is the same, this is just the only difference

# Reading #

## Data Structures: Objects and Arrays ##
* In regards to the wrong inputs leading to right answers, I guess AI could actually parse through your inputs to determine what exactly they are, leading to the right answers

* As a science buff, I like the atom analogy. 'What is the origin of life for computer science' should be the next question lol
 * I suppose that objects could be classified as subcategories on the periodic table

## The weresquirrel ##
* lycanthropy - mental disorder in which the patient believes that he is a wolf or some other nonhuman animal
  * Just an interesting new word

## Data sets ##
* Arrays, Lists, etc

* Exemplified by our previous work:
  ```
  const xyz [1,2,3]
  console.log(xyz[2]) //2
  ```
* Can also do arrayName[i] with a variation of i++ or i+=xyz

* Beginning index is 0:
  ```
  const xyz [1,2,3]
  console.log(xyz[2]) //returns index position 2, which is the value '2'
  ```

* Properties are accessed as such:
  * Access properties by a . or []
  * arrayName.property
  * xyz.length - returns the length of the array
  * xyz.max - returns largest value in array
  * xyz.min - returns smallest value in array

```
const xyz = [
  abc: 123,
  pirate: arr
]
```
* xyz.abc returns //123
* xyz.pirate returns //arr

* THESE ARE ALSO PROPERTIES OF AN OBJECT

__NULL HAS NO PROPERTIES__
__NEITHER DOES UNDEFINED__(per Chat GPT)

* If you want to access a property, such as an index position like '2', you HAVE to use []

* Arrays also have a length property

## Methods ##
> I think the term 'Methods' was the most confusing concept for me when I first began programming, and I am not entirely sure why. It was between that and the unexplained interchange of parameters/arguments. Now, I have no issue with them
> but I thought that this would be worth noting.

* arrayName.push(ValueToAdd) - adds a value
* arrayName.push(ArrayName) - lists array items in order
* console.log(sequence.pop()) - deletes last item in array

* has ToUpper and ToLower just like C# and SQL

* "A stack, in programming, is a data structure that allows you to push values into it and pop them out again in the opposite order so that the thing that was added last is removed first"
 * Last In - First Out
 * .peek will let you see the last item in, aka top of the stack

## Objects ##

<img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgPqf97UYVC5UfV29PmS_ACb6vN801V36TmF9cpb0w0xjc_MlkYWexTT59GpGExNsZaxWsiak2mlpShy21c15mOZUWR0vqu-d2vcm-auyxgUuDK25NGyiW3LiuSVg2E620XpcY-iWjkgV99/s1600/scary-squirrel-pictures-2.jpg" alt="Scary Squirrel" width="200" height="150">

* Since we are referencing Ware-Squirrel so much ^^

* Objects are collections of properties, such as arrays

```
let descriptions = {
  work: "Went to work",
  "xyz": "Touched a tree"
};
```
* to call "xyz, we must do descriptions["xyz"] as the name is not a valid binding name as it is inside of ""

* reading a property that doesnt exist will return "Undefined"
 * you can assign this value by simply doing arrayName.property = [AddItHere]

* You can call:
  * console.log(arrayName.ItemInArray) //true
  * console.log(arrayName.ItemNotInArray) //false

* To delete a value of an item from array, do:
 * delete arrayName.ItemToBeDeleted
 * This actually only removes the VALUE assigned to ItemToBeDeleted (?)

* To log the keys of an object:
  * console.log(Object.keys(arrayName))

* To assign a new value to an object/add a key:
  * Object.assign(arrayName, {key: newValue)
* I understand that this technically is copying all properties from one object into another, but this was an easier explanation for my note purposes

```
const arrayName = [
  {possibility: ["parameters of this possibility"]
    ItemToBeDetermined:False}
  {possibility: ["parameters of this possibility"]
    ItemToBeDetermined:False}
  {possibility: ["parameters of this possibility"]
    ItemToBeDetermined:True}
]
```
* I am using "Parameters" here a little loosely, but isn't it kind of the same principle? It seems as those items must be true for the validation of True or False to be assigned

```
let object1 = {value: 10};
let object2 = object1;
let object3 = {value: 10};

console.log(object1 == object2);
// → true
console.log(object1 == object3);
// → false

object1.value = 15;
console.log(object2.value);
// → 15
console.log(object3.value);
// → 10
```
* This was interesting, I understand the ability to assign the value of object1 to object2 so that when object1 changes, so does object2; however, it is interesting with the initial output that object1 doesn't equal object3, regardless of them both storing the value of 10

* == compares IDENTITIES not properties
  * This is actually a pretty good explaination and made that example much more clear to me
