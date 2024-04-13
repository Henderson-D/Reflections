## Multi-Paradigm Nature of JS ##
__What Does it mean__
* Multi-paradigm programming is the practice of using different styles of programming in one project to make the most of each style's strengths

* Imperitive JS is essentially writing everything out, exactly what we have been doing for the most part
* OOP - more transformative, easier to make changes
```
class Counter {
constructor(start, end, step){
  this.total = 0
  this.count = count
  this.end = end
  this.step = step
}

calcTotal () {
  while (this.count <= this.end){
  this.total += this.count
  this.count =+ step
}
}
}

const counter = new Counter(0,10,1)
console.log(counter.calcTotal())
```

> This makes perfect sense, actually. 0 is start, ending at 10, incrementing(or stepping) by 1. As long as total is less than or equal to end, it will continue incrementing by the designated step amount after += total and count. This is one of the most understandable examples from AI that I
> have seen, personally.
>
> To change the start, end, and incremental factor, you simply change the arguments being passed through.

* To clarify, OOP is refering to the Object that its the container, designated by this.end having a different value than this.end in another object, hense OOP?

* Really do not want to have more than 3 parameters
```
class Counter {
constructor({start =1, end=10, step=2}){
  this.total = 0
  this.count = count
  this.end = end
  this.step = step
}

calcTotal () {
  while (this.count <= this.end){
  this.total += this.count
  this.count =+ step
}
}
}

const counter = new Counter(start:1, end:10, step:2)
console.log(counter.calcTotal())
```

## Destructuring ##
* Shown Above
* You can set default values and only change one of the parameters
* Largely beneficial in how you can extract variables in a efficient way as well as how you can use the functionality of it to pass more than two arguments through, as shown above
* This and OOP aren't necessarily the correct tool for everything

> The clean code shown does definitely make a difference, it makes sense as to why you would not want more than 2 parameters. I do actually like the "new Counter(start:1, end:10, step:2)" as it is much more readable to come back and see exactly what is being passed through as what
>
> The single object allows the arguments to be much more readable in the future, even as you are writing the code now

> The default values are specified by declaring them in the new Counter(start:1, end:10, step:2). If there is not a new value passed through, these defaults will remain in place. We do have to pass through at least one argument as the lack of anything will return as undefined

## DOM Document ##
* DOM Tree
  * Tree diagram that represents HTML or XML documents
* Document API
  * Allows you to modify DOM tree in any way that you want
* You can call a function by doing onclick-"functionName()"

> I would see us making a reactive website that can be modified directly from the user. You could possibily use use this.name or similar to pass user information to be displayed on the site. You can very obviously also use this to change the entire layout if you were so inclined to do so.
>
> I could also see this being how you could create an instant Dark Mode as well, simply changing color schemes and so forth.

> Reviewing the documentation further, I think the biggest thing for me will be remembering the specifications such as document.doThisAction. I could imagine using this "const para = document.getElementsByTagName("p").item(0)" on a scraper to get specific information from a webpage as well

> Overall, this all makes sense to me, so far. I am actually ready to get back into the web designing aspect of this class as well, the change of pace is definitely nice to keep everything fresh and new!

> The JS fundamentals are used in conjunction with HTML fundamentals to get a desired change on the webpage when the item you have set to trigger the change is indeed triggered. This is interesting and would definitely be fun to use in conjunction with TailWind CSS as well. I can see that
> we are likely headed to make a reactive webpage and I will likely begin exploring what changes would interest me the most.
