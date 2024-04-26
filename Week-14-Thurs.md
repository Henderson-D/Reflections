## Beginning Notes ##
> Last week, I had completed some of the homework in a way that wasn't exactly what you were looking for, accidentally. I did undo this work and began fresh this week, so please ignore any early on committs, unless you feel like looking at them lol

## Importing ##
Writing an import statement
```
import * as data from "./src/data"
//* designates as "all" as in SQL
```

__Destructured Version__
```
import {Belts, Champions} from "./src/data"
```

## Filter ##
```
const arrayName = ['xyz', 'abc', 'jbg']

const variName = arrayName.filter((param) => word.length > 6)
//only filters through strings with over 6 character positions
//word.length>6 is a true/false statement,

doThis => ifThis.isTrue
```

> I completely understand the .filter now after doing this assignment and seeing the !===. For whatever reason, that made something in my head click as far as we are filtering out (returning) the items without the term that
> we are filtering for.

> I did also review your code in the video/lib.js as well. I was interested in how ".includes" works in JS and it works essentially exactly how I expected it to.

* Vitest is testing framework
  * "test": "vitest"
  * write the test first, watch it fail, then write function code. This ensures that the test passing is actually valid
  * ``` test("nameOfFunctionTesting", () => {
    // Arrange
    const name1 = [];
    const name2 = [];
    const filterTerm = [];

    const expected = {
      intended ouput here
    }
    
    //Act
    const result = functionName({params})
    //Check if the function correctly removes the corresponding items
    validating code here
   })
  ```
* If the key and value are the same thing, you can simply do (item1, item2, item3) instead of (item1:xyz, item2:xyz, item3:xyz)

```
@typedof {type} Name
@property {type} Name
```
* Interesting that JS is picky here, but not when declaring items otherwise

```functionName.terms1, terms1[index]``` assigns a new value to terms1

> I would definitely need to review some of these items a little more; however, this was not _insanely_ advanced as I have seen some of this already.

__Review__
abc = {...xyz} is related to destructuring and assigning the values of xyz to abc _SPREAD OPERATOR_, Creates new object

> Overall, this was not insanely out of reach and a lot of it made perfect sense after doing some additional reading/research on my end to review some more examples/additional explanations. I do know that this did not make entirely a lot
> of sense to some others, as they reached out for some additional explanation and I provided some brief summarization style assistance that made it click for the most part where they were able to continue.

> I would like to tutor for this class; however, I am currently weighing my professional schedule and lack of time as a very obvious down side to this. If I am able to, I will definitely attempt to if the window is still open. If not, then
> maybe some other time.

> I hope to continue learning some new ideology on how to complete some of these projects. I believe it may be helpful to some of the other people to do a "here is our objective, here is our thought process, here is how we translate that over to psuedo-code, here is how we translate that to code." It is definitely not possible to teach critical thinking, but some sort of professional problem solving skills for some other students may definitely be helpful.
