## Fix Template Repo to Include .vscode Directory ##
* Be in correct repo
* .vscode was ignored
  * This means extensions and settings were not actually committed to GitHub
#### Make sure we have .vscode, extensions.json, and settings.json, then copy and paste the contents of settings/extensions files ####
* In real code, you mostly don't want to overuse console statements
* Semi-colon - automatically inserted if they are not present, are optional but corrected by eslint or prettier formatting
* Semi-colon is like a period, an end of a thought. Not fully needed, but it is proper to use them. USE THEM
##### CANNOT USE LINE BREAKS WHEN DOING RETURN #####
* Block of code - group of code contained within {}
##### CONST #####
* = is an assignment operator, functions from right to left
  * const 1[sum] = 2[addNumbers(5,10)];
  * grabs information to be used[2] then assigns it to declared variable[1]
  * Kind of like how SQL uses FROM before SELECT
* const [name] = [data you want to store in memory]

> Interesting that you can do "sum = xyz;" and exclude const. I agree, this would be a terrible error and relatively unreadable in the future. What does JavaScript define sum as in this case as far as data type,
> when it is not declared by us? Does it default to const?

# NEXT TO DO: Re-Read the Eloquent JavaScript Example Codes #
