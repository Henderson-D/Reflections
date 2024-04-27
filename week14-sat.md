# Sort() Research #
* Sorts elements of an array _in place_ and returns the reference to the same array, sorted
* Default sort is in asc order
* will return ``` 1, 10000, 2, 3, 400000 ```
* ```
  const arrayName = [a, b, c, d]
  arrayName.sort()
  console.log(arrayName) //a, b, c, d
  ```
### Parameters for Sort() ###
(a = 1st element for comparison) (b = 2nd element for comparison)
* first and second element will never be undefined
* negative value indicates that a should come __before__ b
* positive value indicates that b should come __before__ a
* === value indicates to keep original order of a and b
* Zero or NaN indicates that a/b are considered equal
* (a,b) => a-b sorts numbers in ascending order
  * presumably, (b,a) => b-a sorts numbers in descending order
* sorted according to each character's Unicode code point value
> Per ChatGPT, "For example, if you have the string "hello", you can sort it according to Unicode code point values as follows:
>
> 'e' (Unicode code point 101)  
> 'h' (Unicode code point 104)  
> 'l' (Unicode code point 108)  
> 'l' (Unicode code point 108)  
> 'o' (Unicode code point 111)  
> So, the sorted string would be "ehllo".  

* "banana" comes before "cherry". In a numeric sort, 9 comes before 80, but because numbers are converted to strings, "80" comes before "9"
  > b before c, 8 before 9

> When messing with the code on the website:
> ```
> const months = ['abc', 'abd', 'Feb', 'Dec'];
> months.sort();
> console.log(months);
> // Array ["Dec", "Feb", "abc", "abd"]
> ```
> really confused me, this is in really no order at all, aside from abc, abd. However, I get that it is using unicode values now. D and d have different unicode values. I would probably want to do .toLowerCase and then compare the values, no?
>
> I mean, I get the comparison between the values as they are, but no typical individual would sort the objects as it initially did

```
function compareFn(a, b) {
  if (a<b) {
    return -1; //a comes before b
  } else if (a>b) {
    return 1; //a comes after b
  }
  // a must be equal to b
  return 0;
}
```
## What does it mean when it mentions "in place"? ##
> It essentially means that we are sorting the items inside the actual array. Once they are sorted, you can call the arrayName and it will output the sorted result.

# toSorted() Research #
* Essentially just .sort() but creates a copy rather than sorting the initial array
* Must be stored in a variableName to call back.

```
const months = ["Mar", "Jan", "Feb", "Dec"];
const sortedMonths = months.toSorted();
console.log(sortedMonths); // ['Dec', 'Feb', 'Jan', 'Mar']
console.log(months); // ['Mar', 'Jan', 'Feb', 'Dec']

const values = [1, 10, 21, 2];
const sortedValues = values.toSorted((a, b) => a - b);
console.log(sortedValues); // [1, 2, 10, 21]
console.log(values); // [1, 10, 21, 2]
```

## What's the Difference? ##
> The difference is that sort() sorts the original array and can be accessed by calling that original arrayName; however, toSorted() is assigning the sorted values of one array to another newVariableName and it can be accessed by calling the newVariableName rather than
> the original arrayName.
