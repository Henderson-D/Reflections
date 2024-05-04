## General Thoughts ##
> I honestly had spent a good time with the passing code to actually get it to pass. Really, for no reason. I went back, reviewed the video, my code was exactly the same, just on different lines due to my
> extensions saving it differently. However, once I reorganized it exactly like the code, it worked perfect. I am not entirely sure why that is.

### Reduce ###
* Returns a single value, total of all other values it is being applied to
* (Accumulator, currentValue) is essentially total += newValue. Accumulator holds a value and adds the next value to its current value until it reaches the end
* [] _references_ the value assigned in key1 and key2's position
* > My initial explanation was going to be similar: Like a parameter passes through the value in that parameters position, this is simply passing through the value in that position. This may not be the
> 100% accurate description, but it was my initial thoughts, similar enough that it clicked when you mentioned that it is _referencing_ the value in the key1/key2 position

> The tests themselves are not entirely confusing, after seeing your block of code for testing names with different variations of spaces/special characters it is evident that you most are changing the input
> and the expected output, it looked pretty simply. However, it would probably be more confusing when writing tests for more complicated code, that is the aspect that I probably need more practice with.
