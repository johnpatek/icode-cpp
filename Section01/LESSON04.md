# Control Statements and Operators

We have learned about using keywords and identifiers to make variables
and functions, but there are two features that can use with them to make
our code even more powerful.

## Control Statements

Control statements, sometimes called flow control, are statements we 
can use to control how our code runs based on certain conditions.

### If, Else, and Else If

In C++, we can use the keyword `if` along with a `bool` value to create
a block of code that only executes if the value is `true`. Sometimes, 
we want to create another block of code when the `if` statement has a 
value of `false`. These blocks are called `else` statements, and they
can only be used following an `if` block. For some special cases, we
want the `else` block to check a second condition, in which case we
use an `if else` block, which is only checked if the first `if` has a 
value of `false`. Below is a simple function that uses `if`, `else if`,
and `else` to execute our code based on the value passed to the function.

```c++
void print_sign(int val)
{
    if(val > 0)
    {
        std::cout << "positive number" << std::endl;
    }
    else if (val < 0)
    {
        std::cout << "negative number" << std::endl; 
    }
    else
    {
        std::cout << "zero" << std::endl;
    }
}
```

It's important to note that the values we put inside an `if` statement 
do not have to be variables or hard coded values. In this case we use
`val > 0` and `val < 0`, which are expressions, whose `true`/`false`
values are not known until the code is run. An `if` statement can use 
any provided `bool` value, whether it is a variable, expression, or 
even another function, as we will see in our project.

### While and Do While

### For

A for loop is a block of code that will repeat based on a counter. We
should use it when we can easily determine how many times a block of
code needs to be reapeated. See the example below:

```c++
void print_dozen()
{
    for(int count = 0; count < 12; count++)
    {
        std::cout << (count + 1) << std::endl;
    }
}
```

Inside of a `for` statement, we have 3 statements:

1. We declare the counter `int count = 0;`
2. We provide an expression that will tell the loop when it needs to
stop. In this case `count < 12;` tells the loop to repeat until `count`
is 12.
3. We tell the loop how to modify the counter each time after the loop
runs. Our expression `count++` will increase the counter by 1 on each
iteration.