# Is it Prime?

In this project, we will make a simple program to check if a number is
prime and print the result.

## Code

Here is the code:

```c++
#include <iostream>

static bool is_prime(int value)
{
    // return true iff value is prime
    return false;
}

static void print_is_prime(int value)
{
    // print if value is prime or not
}

int main()
{
    print_is_prime(4); // this should print "4 is not prime"
    print_is_prime(5); // this should print "5 is prime"
    return 0;
}
```

### Implement `is_prime`

The `is_prime` function should take `int val`, and return true if it
is prime, and false if it is not prime.

HINT: You can add `#include <cmath>`, which has the `sqrt` function. If
the value of `val % x == 0` for any `x` value [2, sqrt(val)], then val
is not prime.

### Implement `print_is_prime`

This function should take `int val` and use the `is_prime` function
to print if it is prime or not.

HINT: use an `if` statement and `std::cout`.

## Testing

In order to verify our solution is correct, we need to compile and run
our code. If the output is:

```bash
4 is not prime
5 is prime
```

Then you are done!