Source code (0 and 1) ``\to `` compiler ``\to`` machine code (what we write)

How to evaluate the quality of code:
1. Is it correct?
2. Design
3. Style (aesthetics of your code)

Terminal window provides Command Line Interface (CLI which is in contrast with a Graphical User Interface: GUI) and the former is more powerful and efficient.

File explorer; Activity bars

The file name used to be lowercase.

Hello.c and hello (machine code)

Escape sentence

String of text must be on the same line

```
include <stdio.h>
```
Like adding a library. So called head file.
This head file contain enough information about all of the functions in what’s called the Standard I/O library. (file)

[manual pages](manual.cs50.io)
[stdio.h](manual.cs50.io/#stdio.h)
[printf](manual.cs50.io/3/printf)
cs50.h

assignment:
```
string answer = get_string(“What’s your name? ”);
printf(“hello, %s\n”, answer);
```
```
printf(“I get 100%%”)
```
bool char double float int long string…

```
if (x < y)
{
    printf(“x is less than y\n”);
}
else if (x > y)
{
    printf(“…”)
}
else
{
    printf(“x is equal to y\n”);
}
```

single quote for char; double quote for strings

```
if (c == ‘y’ || c == ‘Y’)
{

}
```

```
#include <stdio.h>

int main(void)
{
    for (int i = 0; i < 3; i++)
    {
     printf(“meow\n”);
    }
}
```
```
i = i + 1; i += 1; i++;
```
```
int i = 3;
while (i > 0)
{
    printf(“meow\n”);
    i -= 1;
}
```
```
#include <stdbool.h>;
```

Linux is very often used on servers nowadays

cd cp ls mkdir mv rm rmdir

```
const int n = 5;
```

```
// Get size if grid
int n;
do 
{
    n = get_int(“Size: “);
}
while (n < 1);
```
pseudocode
```
#include<stdio.h>

int get_size(void);
void print_grid(int size);

int main(void)
{
    int n = get_size();
    print_grid(n);
}

int get_size(void)
{
    int n;
    do
    {
        n = get_int(“Size: “);
    }
    while (n < 1);
    return n;
}

void print_grid(int size)
{
    …
}
``` 

int: 32bits (the biggest number: 2147483647, half of the number is negative)
integer overflow

long 
```
printf(“%li\n”, x + y);  
```
truncation
```
printf(“%f\n”, x / y);
```
type casting
```
float z = (float) x / (float) y;
```
floating-point imprecision
```
printf(“%.20f\n”, z);
```
double (64bits) for more precision

``1999 \to 1900``
19 January 2038 (seconds 32bits) = 13 December 1901                    