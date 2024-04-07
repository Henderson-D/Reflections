## Genereal Thoughts About Code Examples ##

* Here are a few of my examples:
> Please note that I am involved in Army training this weekend; thus, this work was completed offline and will unfortunately be committed as a block to index.js, rather than as proper commits.
> There really wasn't much that I could do about this.

## Example 1 ##
```
const nameAge = (name, age) => {
	const message = `Hello, ${name}! You are ${age}`
	return(message)
}
console.log(nameAge('Derrick', 22))
```
## Example 2 ##
```
const todayDate = () => {
const currentDate = new Date();
 
const year = currentDate.getFullYear();
const month = currentDate.getMonth() + 1;
const day = currentDate.getDate();

return(`${year}-${month}-${day}`);
}

const nameAge = (name, age) => {
	const message = `Hello, ${name}! You are ${age}`
	return(message)
}

const customMessage = (greeting, date) => {
    const welcomeMessage = `${greeting}` + ` and today is ${date}`
    return welcomeMessage
}

console.log(customMessage(nameAge('Derrick', 22), todayDate()))

```
## Example 3 ##
```
const arrayName = [
    123
];

function functionName(array) {
    return (prefix) => `${prefix} ${array[0]}`;
}

const variableName = functionName(arrayName);
console.log(variableName("Prefix"));

returns //"Prefix" araryName.item
```
## Another copy of the football score program ##
```
const message = "The score is: ";

while (true) {
    let totalScore = 0;

    for (let i = 0; i < 70; i++) {
        const point = parseInt(prompt('What point was scored? '));
        
        const newScore = (score) => {
            if (score % 6 === 0 || score % 3 === 0 || score % 2 === 0) {
                totalScore += score;
                return totalScore;
            } else {
                return "Not a valid point";
            } 
        };
        
        const messageScore = (scoreIs, addedScore) => {
            return `${scoreIs} ${addedScore}`;
        };

        console.log(messageScore(message, newScore(point)));
    }
}
```

## Begin Reflections ##
> I do generally believe that I understood these new concepts; however, I do hope that I implemented them properly. I am doing Army activities this weekend, unexpectedly, and I did not always have access
> to the internet, where my Google Sheets notes are. I suppose that I should localize those. However, I did put in quite a bit of work on these examples, especially the final footballScore example. I tried
> to pass functions as arguments, while pulling functions out of functions. I also used the opportunity to use a prompt, something that I haven't attempted in JS yet. I did also implement a simple while(true)
> loop simply just to get this code to function as a loop. I will admit, the final concept of pulling functions from functions is a little fuzzy to me, I would definitely appreciate some more explanation on
> this concept. I will definitely do some research on my end as well.
>
> I just went and did another example for closure. It was irritating me that I didn't understand it as well as I should. Correct me if I am wrong, but to simplify:

* You are creating an initial "host" function
* Inside of this function, there is another declared function, nested
* You can pass the nested function through a return statement, possibly using a parameter from the initial function as another parameter, or similar
* When you call the inital function, since you are returning the second, you are essentially passing the value of the nested function through the first
* While I know that I am not "pass/by copy"-ing the nested function, it is just easier to explain that

* Is this correct?
