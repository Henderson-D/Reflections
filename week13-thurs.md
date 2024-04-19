## General Notes, Let's Read ##
* BOM - Browser Object Model
 * Provides objects to interact with the web browser
*BOM key factors are:
 - Window Object: such as browser window
  - like popup windows
 - Nav Object: provides info about brower, such as name, version, operating system
 - Location Object: URL, path to specific location, provides methods to redirect browser to another URL
 - History Object: Provides methods to interact with browsers session history, pages that were visited in that specific tab, like back arrow
 - Screen Object: Provides info about screen size, resolution
 - Document Object: part of the DOM, but document object is also assessible through BOM, allows scripts to manipulate the page
> BOM would just refer to the more indepth sections that are not as often thought about. BOM directly relates to the term "Digital Fingerprint" to me in terms of screen size, reviewed sites, and other specific topics.

* DOM - Document Object Model (Meaning HTML document)
 * Provides objects to interact with the document structure, style, and content
*__Key Factors:__
 * Nodes: a building block, like ```<p> or <div>```, etc
 * Element Nodes: Much like the above
 * Text Nodes: Represents the text __INSIDE__ of elements, <p>Like This</p>
 * Attributes: Can include things like ID's, classes, src, href, etc
 * Document: HTML or XML (LOL at the not worrying about XML comment, I thought the same thing initially)
> Once Document was explained, this all made perfect sense to me, as initially, I had forgotten what exactly it was referencing

## BOM and DOM Demo ##
__Console__
* CNTL+SHFT+I for windows devop tools
* Anything doing in browser is part of window.(insertHere)
* Looks pretty straight forward for this, I was not expecting print to function like that for whatever reason

__Elements__
* .textContent will tell you content of the specific element
* document.querySelector(".name_of_class")
* To get direct child, you can do ```document.querySelector(".name_of_class" > desiredChild)```

__To Change Functionality of Something__
```
variableName.addEventListener("type of event", functionName)
```
> I have "Cheated" and reviewed quite a few videos about this exact topic, one being here:
<a href="https://www.youtube.com/watch?v=x5trGVMKTdY&t=2715s" target="_blank">Watch the Video</a>
> It should automatically be on that time stamp for ~45 mins, where it directly talks about this

> This is probably the seciton that I am most interested in to be honest as I have reviewed countless videos regarding HTML, CSS, JS, C# and so forth from random school lectures, usually Harvards free classes.

* ('tag')
* (#id)
* (.class)
