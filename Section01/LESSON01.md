# Introduction

Start here!

## Hello World

Like most programming languages, the first thing to do is write a simple
"Hello, World!" program:

```c++
#include <iostream>

int main()
{
    std::cout << "Hello, World!" << std::endl;
    return 0;
}
```

Now, let's break it down and see what each part of this code does:

```c++
#include <iostream>
```

The `#include` directive tells the compiler that we need to access some
code that is outside of our program, and `<iostream>` is the code we will
be accessing.

```c++
int main()
```

All C++ programs (and C programs) begin in a function called `main()`,
which we refer to as the "entry point" for our program. When our system
starts a new process, it looks for a place to start running, and this
function tells it where to start.

```c++
std::cout << "Hello, World!" << std::endl;
```

This code prints some text to our console. `std::cout` is a stream object
that we use to send data to our console output. The symbol `<<`  tells the
compiler that we will be inserting something into this stream. `std::endl`
is a newline operator, which means that once we are done printing to
`std::cout`, our console output will go to the next line before printing
again.

```c++
return 0;
```

This is the last statement in any C++ program, and it tells the system
that our process is exiting with code 0, which means no errors occurred
during execution.