# Data Types, Variables, and Functions

In this lesson, we will learn about the different types of data we can
handle, how to store that data, and how to create functions that allow
us to have separate blocks of reusable code.

### Data Types

A data type is a keyword or special identifier that tells the compiler
what type of data we want to store. Some of the common data types we
have as keywords include:

+ `bool` - Boolean value, which can be `true` or `false`.
+ `char` - Character value, usually a single byte that can be a single
letter, digit, or symbol, such as `'A'`, `'1'`, or `'+'`.
+ `int` - An integer value.
+ `float` - Floating point value, which is a number that can include a
decimal.
+ `double` - Double precision floating point value, which is a lot like 
`float`, except it takes up twice the memory space to provide an extra
level of precision in our calculations.
+ `void` - This is a special data type that does not hold a value. It
is not especially useful for variables, but it can be very useful for
certain functions.

### Variables

A variable is a data type combined with an identifier that we can use
to store information. This is illustrated in the following:

```c++
int my_variable; // declare variable of int type
my_variable = 5; // use assignment operator to store value of 5
my_variable = 3; // use assignment operator to overwrite with value of 3
```

### Functions

A function is a separate block of code that we can reuse as many times
as we want. See example:

```c++
void my_func(double d)
{
    // do something
}
```

This function can be called using `my_func()` and inserting a value in
the parantheses. The compiler will accept a hard coded value such as 
`my_func(0.5)` or even a variable `my_func(my_double)` as long as the 
variable `my_double` was declared as a `double`.

### Example

```c++
#include <iostream>

static void print_num(int val)
{
    std::cout << "the value is " << val << std::endl;
}

int main()
{
    int num;
    num = 1;
    print_num(num);
    num = 2;
    print_num(num);
}
```