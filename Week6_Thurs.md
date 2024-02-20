# JS Code Video #
* String- "XYZ"
* [____] - a collection of items
  * ["XYZ", "ABC"] would be a collection of strings
* .gitignore - creates a file in which you can place a collection of items that will not be stored in a git repository, eliminating clutter
* .prettierrc {} - essentially just uses defaults
* package.json - lists out items that you are using in your project, such as eslint and prettier

## Code Portion ##
### Video 1 ###
* Create a new file, add to repo
* function is a keyword,
> function descriptiveName (parameter1,parameter2)
> {return |what you want to be completed placed here|} ; 
> (Names are camelCased, and are not single letter variables, somewhat descriptive of what the variable is)
### Video 2 ###
> The goal is to:  
1. place keyword
2. give it a name
3. insert place holders
4. return code to be run

* The above does not actually do anything, other than create that function to be used later. The function must actually be CALLED
  
* const descriptiveConstName = functionName(argment1, argument2);
  * This is storing the result of the function in a variable, waiting to be called later
  * A variable is essentially a PLACEHOLDER of whatever information it holds
  * We will stick with "const" 80% of the time
  
* argument1 and argument2 will take the place of parameter1 and parameter2, accordingly. parameter1 and parameter2 are simply PLACEHOLDERS

* console.log("Example sentence here:", descriptiveConstName);

* Looks like the syntax is similar to C# in the sense that each line is ended with ; aside from {}, just like C#

* node fileName.js
  * Will run the code inside of the file
  * the console.log("XYZ") is what is actually getting us the output, making it visible

* If you were to put the constName inside of the "", it would put the constName as plain text, not the intended output

* To comment DO:
  > // intended comment here //

* "Unexpected console statement"
  *   THIS IS OKAY TO SEE FOR NOW - Just means that we aren't actually sending the information somewhere else, we are just printing it

# General Reflection #

> I did think this was easy to follow, much more so than the Git Bash at the beginning. I am at least familiar enough with how it looked, as I am referencing some items to C#. I am keeping in mind that this is surely not much like C#, but
> for now it is helping me keep everything relevant and straight. My initial idea of JavaScript seems to be a mix of C#-ishness and HTML intertwined. Maybe this is incorrect, but this is my hypothesis. I think there has to be some similarity
> amongst most programming languages, but still distinct differences and differing use cases.

> I do believe that I understand the concepts as well. Much like other languages and even basic math, you simply create a variable and store information inside, then use it later. The most difficult part for me, for whatever reason, is
> remembering the distinct differences between "parameters" and "arguments." I understand that a parameter is a placeholder for a future argument, but for whatever reason this slips my mind when I am in the moment. So, I will refer
> back to these notes when the inevitable brain-slip occurs.

> The easiest part was a part that was not discussed, the ending of each line with ";", aside from the select few where that is incorrect syntax, such as {}. Also, I like that you can run this directly in GitBash as well, that is very
> helpful that you do not have to go anywhere else other than VS Code and Git Bash, I believe at least. I am wondering how inputs function in JavaScript currently. As much as I would like to look it up, I am not going to as I want to
> learn this at whatever pace you set. There are some things that I am sure I could harmlessly pickup along the way on my own, but I do not want to add unneeded confusion on my end.
