# Notes by Krishna Rawat
# Looping Statements in C

## Definition and Types
- Looping statements execute a set of statements repeatedly until a condition becomes false.
- Two main types:
  1. Entry controlled (pre-test): condition checked before loop execution (while, for)
  2. Exit controlled (post-test): condition checked after loop execution (do-while)

## While Loop
- Syntax: 
  ```c
  while (condition) {
      statement(s);
      incrementation;
  }
  ```
- Entry controlled loop

## Do-While Loop
- Syntax:
  ```c
  do {
      statement(s);
  } while (condition);
  ```
- Exit controlled loop
- Always executes at least once

## For Loop
- Syntax:
  ```c
  for (init; condition; increment) {
      statement(s);
  }
  ```
- Entry controlled loop
- Combines initialization, condition, and increment in one line

## Key Concepts
- Loop control expression: condition that controls the loop
- Initialization: sets starting value for loop variable
- Condition: determines when loop should continue or terminate
- Increment/Decrement: updates loop variable after each iteration

## Applications
- Printing sequences of numbers
- Calculating factorial
- Finding Fibonacci series
- Checking for palindromes or Armstrong numbers
- Calculating sums and averages

# Nested Loops in C Programming

## Definition:
- A nested loop is a loop inside another loop. 
- C programming supports nesting any type of loop inside another loop.

## Syntax:
```c
outer_loop
{
    inner_loop
    {
        // Inner loop statement/s
    }
    // Outer loop statement/s
}
```

## How Nested Loops Work:
- The inner loop runs only when the outer loop condition is true. 
- If the condition in either loop turns false, control exits the respective loop.

## Examples:

1. **Multiplication Table**: 
    - A program using nested loops to print a multiplication table from 1 to 5.
    ```c
    #include <stdio.h>

    int main()
    {
        int i, j;

        for (i = 1; i <= 10; i++)
        {
            for (j = 1; j <= 5; j++)
            {
                printf("%d	", (i * j));
            }
            printf("\n");
        }

        return 0;
    }
    ```

2. **Pattern Printing**:
    - Using nested loops to print repeated patterns (e.g., `********`).

## Summary:
- The number of iterations in a nested loop equals the outer loop’s iterations multiplied by the inner loop’s iterations.
- Any number of loops can be nested, with no theoretical limit.

# Jump Statements in C Programming

## Definition:
- Jump statements are used to modify the behavior of loops and conditionals by changing the flow of control within a program.

## Types of Jump Statements:

1. **Break**: 
    - Terminates the loop or block and transfers control to the next statement.
    ```c
    break;
    ```

2. **Continue**: 
    - Skips the rest of the loop iteration and jumps to the next iteration.
    ```c
    continue;
    ```

3. **Goto**: 
    - Transfers control to a labeled part of the program.
    ```c
    goto <label>;
    ```

4. **Return**: 
    - Ends a function and optionally returns a value to the calling function.
    ```c
    return <expression>;
    ```

## Examples:

1. **Break Statement**:
    ```c
    #include <stdio.h>

    int main()
    {
        int i;
        for(i = 1; i <= 15; i++)
        {
            if(i == 10)
                break;  // Exit loop when i equals 10
            printf("%d\n", i);
        }
        return 0;
    }
    ```

2. **Continue Statement**:
    ```c
    #include <stdio.h>

    int main()
    {
        int i, j;
        for(i = 1; i < 3; i++)
        {
            for(j = 1; j < 5; j++)
            {
                if(j == 2)
                    continue;  // Skip iteration when j equals 2
                printf("%d\n", j);
            }
        }
        return 0;
    }
    ```

3. **Goto Statement**:
    ```c
    #include <stdio.h>

    int main()
    {
        int i;
        for(i = 1; i < 5; i++)
        {
            if(i == 2)
                goto there;
            printf("%d\n", i);
        }
        there:
        printf("Two");
        return 0;
    }
    ```

4. **Return Statement**:
    ```c
    #include <stdio.h>

    char func(int ascii)
    {
        return ((char)ascii);  // Return character value of the ASCII code
    }

    int main()
    {
        int ascii;
        char ch;
        printf("Enter any ASCII value in decimal: ");
        scanf("%d", &ascii);
        ch = func(ascii);
        printf("The character is: %c", ch);
        return 0;
    }
    ```

## Summary:
- **Break**: Used to terminate loops or switch cases.
- **Continue**: Skips to the next iteration in a loop.
- **Goto**: Jumps to a labeled section in the code.
- **Return**: Ends function execution and optionally returns a value.

# Arrays in C Programming

## Definition:
- An array is an ordered set of similar data items stored in consecutive memory locations. All elements in an array have the same data type and can be accessed using a common name.

## Array Declaration:
- **Syntax**: 
    ```c
    data_type array_name[size];
    ```
- **Example**: 
    ```c
    int a[5];
    ```

## Array Initialization:

### 1. Compile Time Initialization:
- **Initializing all elements**: 
    ```c
    int a[5] = {10, 15, 1, 3, 20};
    ```
- **Partial initialization** (remaining elements are set to 0):
    ```c
    int a[5] = {10, 15};
    ```
- **Initialization without size**:
    ```c
    char b[] = {'C', 'O', 'M', 'P', 'U', 'T', 'E', 'R'};
    ```
- **String initialization**:
    ```c
    char b[] = "COMPUTER";
    ```

### 2. Run Time Initialization:
- Arrays can be initialized during program execution using loops and user input.
    ```c
    int x[3];
    scanf("%d %d %d", &x[0], &x[1], &x[2]);
    ```

## Examples:
1. **Program to take 5 values from the user and store them in an array**:
    ```c
    #include <stdio.h>

    int main()
    {
        int values[5];
        printf("Enter 5 integers: ");
        for(int i = 0; i < 5; ++i) 
        {
            scanf("%d", &values[i]);
        }

        printf("Displaying integers: ");
        for(int i = 0; i < 5; ++i)
        {
            printf("%d\n", values[i]);
        }

        return 0;
    }
    ```

2. **Program to find the average of n numbers using arrays**:
    ```c
    #include <stdio.h>

    int main()
    {
        int marks[10], i, n, sum = 0, average;
        printf("Enter number of elements: ");
        scanf("%d", &n);

        for(i = 0; i < n; ++i)
        {
            printf("Enter number%d: ", i + 1);
            scanf("%d", &marks[i]);
            sum += marks[i];
        }

        average = sum / n;
        printf("Average = %d", average);

        return 0;
    }
    ```

## Summary:
- An array is a collection of data items of the same type, accessed using a common name.
- A one-dimensional array behaves like a list.

# Strings in C Programming

## Definition:
- A string in C is an array of characters terminated by a null character (`'\0'`).
- Strings are enclosed in double quotes, while characters are enclosed in single quotes.

## String Declaration:
- **Example**:
    ```c
    char string[10] = "Hello";
    ```

## String Input and Output:
- **Input**: Use `scanf()` with `%s` to read strings, but it stops at whitespace. To read a full line, use `gets()`.
    ```c
    gets(name);  // Read a full line of text
    ```
- **Output**: Use `puts()` to display the string.
    ```c
    puts(name);  // Display the text
    ```

## Concatenation of Strings:
- Use `strcat()` to concatenate two strings.
    ```c
    strcat(s1, s2);  // Concatenate s2 to s1
    ```

## String Functions:
- C provides several functions in the `<string.h>` library for string manipulation, including:
    - `strlen()` to find the length of a string.
    - `strcpy()` to copy one string to another.
    - `strcat()` to concatenate two strings.
    - `strcmp()` to compare two strings.

## Summary:
- A string is a sequence of characters stored in a character array.
- String manipulation is handled using functions from the `<string.h>` header.

# Functions in C Programming

## Definition:
- A function is a block of code designed to perform a specific task.
- Functions help modularize the program by breaking down complex tasks into smaller, manageable parts.

## Types of Functions:

1. **Standard Library Functions**:
   - Predefined functions available in C, such as `printf()` and `sqrt()`.
   - These are included in header files like `<stdio.h>`, `<math.h>`.
   - Example:
     ```c
     printf("Hello world");
     ```

2. **User-defined Functions**:
   - Functions created by the programmer to perform specific tasks.

## Advantages of Using Library Functions:
- They are tested and reliable.
- Optimized for performance.
- Save development time.
- Portable across different systems.

## String Functions in C:
C provides several string handling functions, such as:
- `strcpy()`: Copy one string to another.
- `strlen()`: Calculate the length of a string.
- `strcmp()`: Compare two strings.

## Examples:

1. **Finding the Square Root**:
   ```c
   #include <stdio.h>
   #include <math.h>
   
   int main() {
       float num, root;
       printf("Enter a number: ");
       scanf("%f", &num);
       root = sqrt(num);
       printf("Square root of %.2f = %.2f", num, root);
       return 0;
   }
   ```

2. **Comparing Two Strings**:
   ```c
   #include<stdio.h>
   #include<string.h>
   
   int main() {
       char a[100], b[100];
       printf("Enter the first string
");
       gets(a);
       printf("Enter the second string
");
       gets(b);
   
       if(strcmp(a, b) == 0)
           printf("Entered strings are equal.
");
       else
           printf("Entered strings are not equal.
");
   
       return 0;
   }
   ```

## Summary:
- Functions help organize code into modular blocks.
- There are both standard library functions and user-defined functions.
- C offers built-in string handling functions in the `<string.h>` library.

# User-Defined Functions in C Programming

## Definition:
- A user-defined function is a block of code that performs a specific operation and can be called when needed.
- It helps in organizing large programs by dividing them into smaller blocks.

## Components of a Function:
1. **Return Type**: Specifies the data type of the value returned by the function. If no value is returned, the return type is `void`.
2. **Function Name**: Describes what the function does, following variable naming conventions.
3. **Parameters**: Inputs provided to the function.
4. **Local Variables**: Variables declared within the function.
5. **Function Body**: The block of code that performs the task.
6. **Function Declaration**: Declares the function's name, return type, and parameters to the compiler.

## Types of User-Defined Functions:
1. **No arguments, no return value**:
    - Example:
    ```c
    void functionName() {
        // Function code
    }
    ```
2. **No arguments, return value**:
    - Example:
    ```c
    int functionName() {
        // Function code
        return result;
    }
    ```
3. **Arguments, no return value**:
    - Example:
    ```c
    void functionName(int a, int b) {
        // Function code
    }
    ```
4. **Arguments, return value**:
    - Example:
    ```c
    int functionName(int a, int b) {
        // Function code
        return result;
    }
    ```

## Example: Function to Compare Two Numbers
```c
#include<stdio.h>

int greatNum(int a, int b);

int main() {
    int i, j, result;
    printf("Enter 2 numbers that you want to compare...");
    scanf("%d%d", &i, &j);
    result = greatNum(i, j);
    printf("The greater number is: %d", result);
    return 0;
}

int greatNum(int x, int y) {
    if(x > y) {
        return x;
    } else {
        return y;
    }
}
```

## Summary:
- A function consists of a declaration, function body, and a call.
- Every C program must have at least one function, typically the `main()` function.
- Local variables inside a function are destroyed when the function exits.
- Arguments passed to a function are passed by value.

# Parameter Passing and Calling Functions in C Programming

## Parameter Passing in C:
- **Formal Parameters**: Variables declared in the function prototype or definition.
- **Actual Parameters**: Variables or values passed to the function when calling it.

## Ways to Pass Parameters:

1. **Call by Value**:
    - The actual parameter values are copied to the formal parameters.
    - Changes made inside the function do not affect the actual variables.
    - Example: Swapping two numbers using call by value.
    ```c
    void swap(int x, int y) {
        int temp = x;
        x = y;
        y = temp;
    }
    ```

2. **Call by Reference**:
    - The actual and formal parameters refer to the same memory location.
    - Changes made inside the function affect the actual variables.
    - Example: Swapping two numbers using call by reference.
    ```c
    void swap(int* x, int* y) {
        int temp = *x;
        *x = *y;
        *y = temp;
    }
    ```

## Examples:
1. **Program to Find the Square of a Number**:
    ```c
    float square(float x) {
        return x * x;
    }
    ```

2. **Program to Swap Two Numbers Using Call by Value**:
    ```c
    void swap(int x, int y) {
        int temp = x;
        x = y;
        y = temp;
    }
    ```

3. **Program to Swap Two Numbers Using Call by Reference**:
    ```c
    void swap(int* x, int* y) {
        int temp = *x;
        *x = *y;
        *y = temp;
    }
    ```

## Summary:
- A function includes a declaration, function body, and function call.
- Function calls can either be by value or by reference.
- Ordinary variables in a C function are destroyed when the function exits.
- Arguments passed by value do not change, while those passed by reference can change.

# Recursive Functions in C Programming

## Definition:
- A recursive function is a function that calls itself, either directly or indirectly, to solve a problem.
- It must include an exit condition to terminate the recursion.

## Example 1: Factorial of a Number
```c
int factorial(int number) {
    if (number == 1) 
        return 1;  // base case
    else
        return number * factorial(number - 1);  // recursive case
}
```

## Example 2: Printing First 50 Natural Numbers
```c
void printNumbers(int n) {
    if (n <= 50) {
        printf("%d ", n);
        printNumbers(n + 1);
    }
}
```

## Macros:
- A macro is a preprocessor directive defined using `#define` to give symbolic names to constants or expressions.
- Macros can be defined with or without arguments.
- Example:
```c
#define PI 3.14
#define SQUARE(x) (x * x)
```

## Summary:
- Recursive functions call themselves until they reach a base case that stops the recursion.
- Macros are symbolic constants or expressions replaced by their values during preprocessing.

