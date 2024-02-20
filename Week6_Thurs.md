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
