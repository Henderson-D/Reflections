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
