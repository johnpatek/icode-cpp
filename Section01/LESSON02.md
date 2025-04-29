# Keywords and Identifiers

In C++, most of our code will be made up of statements. Each statement
will consist of a combination of keywords and identifiers that will
tell the compiler what we want our code to do.

## Keywords

Keywords are special reserved words that have a specific meaning. The
compiler looks for these keywords and uses them to determine how our 
code will be compiled. Because of their special meaning, we are only
allowed to use keywords for their specific purpose, and the compiler
will throw an error if we use them as identifiers. Some examples of
keywords are `const`, `if`, `int`, `static`, `class`, and `while`.

## Identifiers

An identifier is a word that we use to identify a variable, function,
class, or any other entity we want to use in our code. We can name an
identifier however we want, as long as it meets 3 requirements:

1. It is not a keyword.
2. It is made up of only letters, digits, and underscores.
3. It begins with a letter or underscore.

Some valid identifiers include `myvar`, `_radius`, `line2`.

Some invalid identifiers would be `for`, `1apple`, `#name`.

## Example

Here is some code that uses keywords and identifiers.

```c++
#include <iostream>

int main()
{
    const int radius = 5;
    std::cout << "this circle has a radius of " << radius << std::endl;
    return 0;
}
```

Since we are already familiar with `std::cout`, let's focus on the other
parts of the code.

```c++
const int radius = 5;
```

In this code, we are declaring a variable `radius` and setting its value 
to 5. Let's look at the keywords:

```c++
const int
```

The keyword `const` stands for constant. When we declare a variable with
`const`, we cannot change it after it is assigned. This might seem like
a limitation to our code, but it actually gives the compiler a chance
to make our program faster because it has more options when handling a
value that is known at compile time.

The keyword `int` specifies that this variable will be an integer. This
is necessary information for the compiler so it knows how our variable
needs to be handled in memory.

Now we can look at the identifier:

```c++
radius
```

This satisfies the requirements for an identifier:

- [x] `radius` is not a keyword.
- [x] `radius` is only made up of letters.
- [x] `r` is the first character in the identifier.

In this case we use the identifier `radius` in the next line to 
identify what value we want to print to `std::cout`.