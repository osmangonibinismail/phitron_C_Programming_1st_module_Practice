# 📘 Phitron - C Programming (Module 1)

This repository contains the practice codes from **Module 1** of the Phitron C Programming Course. I'm documenting everything I’ve learned so far, and keeping it here for future reference. The module covers basic C syntax, variable types, input-output, and some foundational concepts.

---

## ✅ What I Learned

### 🖨️ 1. Basic Output with `printf`
📄 **File:** `hello_world.c`
```c
#include<stdio.h>

int main()
{
    printf("hello world\n");
    printf("Hi I am\tOsman Goni");

    return 0;
}
🔤 2. Using Different Variable Types
📄 File: variable_types.c

c
Copy
Edit
#include<stdio.h>

int main()
{
    int num1 = 50;
    float f = 3.1416;
    char c = '@';

    printf("%d\n", num1);
    printf("%.4f\n", f);
    printf("%c", c);
}
✔️ 3. Boolean Variables (stdbool.h)
📄 File: boolean.c

c
Copy
Edit
#include<stdio.h>
#include<stdbool.h>

int main()
{
    bool b = true;
    bool c = false;

    printf("%d\n", b);
    printf("%d\n", c);

    return 0;
}
🚫 4. Integer Overflow
📄 File: int_limit_error.c

c
Copy
Edit
#include<stdio.h>

int main()
{
    int a = 10000000000; // Too large for int, will cause error
    printf("%d", a);

    return 0;
}
🧮 5. Using long long int for Large Numbers
📄 File: long_long.c

c
Copy
Edit
#include<stdio.h>

int main()
{
    long long int a = 1000000000000;
    printf("%lld", a);

    return 0;
}
🧠 6. Working with float and double
📄 File: float_vs_double.c

c
Copy
Edit
#include<stdio.h>

int main()
{
    double f = 222.448565;
    printf("%lf", f);

    return 0;
}
📥 7. Taking Input from User
📄 File: single_input.c

c
Copy
Edit
#include<stdio.h>

int main()
{
    int a;

    scanf("%d", &a);
    printf("%d", a);

    return 0;
}
⚠️ 8. Incorrect Input Formatting (newline issue)
📄 File: multi_input_wrong.c

c
Copy
Edit
#include<stdio.h>
#include<stdbool.h>

int main()
{
    int a;
    float f;
    char c;

    scanf("%d\n", &a);
    printf("%d\n", a);
    scanf("%f\n", &f);
    printf("%.1f\n", f);
    scanf("%c\n", &c);
    printf("%c\n", c);

    return 0;
}
✔️ 9. Correct Way to Take Multiple Inputs
📄 File: multi_input_correct.c

c
Copy
Edit
#include<stdio.h>

int main()
{
    int a;
    float f;
    char c;

    scanf("%d %f %c", &a, &f, &c);
    printf("%d %.2f %c", a, f, c);

    return 0;
}
🔢 10. Input and Output with Large Numbers
📄 File: long_input.c

c
Copy
Edit
#include<stdio.h>

int main()
{
    long long int a;

    scanf("%lld", &a);
    printf("%lld", a);

    return 0;
}
📁 File List

File Name	Description
hello_world.c	Simple output with printf
variable_types.c	Working with int, float, char
boolean.c	Using bool, true, false
int_limit_error.c	Demonstrating integer overflow
long_long.c	Storing large numbers with long long
float_vs_double.c	Printing precise decimal values
single_input.c	Taking a single input from the user
multi_input_wrong.c	Incorrect multi-input formatting
multi_input_correct.c	Correct way to take multiple inputs
long_input.c	Input/output of large integer values
🧑‍💻 Author
Osman Goni

This is part of my C programming learning journey through Phitron. More modules will be added soon inshaAllah.
