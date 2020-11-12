# clean-code

### The Rules of functions

**The functions should do one thing**

`but what's one thing?`


**first**

`They should be small`

**second**

`They should be smaller than that`

### Indenting

smallness also implies:

`1. functions should not be large enough to hold nested structures`

`2. therefore the indent level of a function should not be greater than one or two`

`3. this of course makes the functions easier to read and undrestand`

### Questions

what types of arguments you should never pass to a functions? `booleans`

**Why???**

because if you pass a boolean to a function, there should be an if statement in that function,

`so what to do?`

**separate them, call one of them in true statement and the other one in false, actually break it to `2` separate functions**

**Avoid Switch statements** `because it's hard to manage`

**No Side Effects**

if you call a function and that function causes the system to change the state then that function has a side effect

a function that returns void must have a side effect

and a function that returns a value should not have a side effect (command and query separation)

prefer exceptions to return error code

Don't repeat your self (DRY)

**How to avoid this ?**

You can make that nice structured code a function and then pass an argument to that function.


# What is the purpose of a comment ?

`is to explain the purpose of the code, if the code can't`

But today's languages are so much better that we can write code, that can explain itself clearly.
