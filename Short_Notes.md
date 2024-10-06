### Looping Statements:
- **Entry Controlled Loops**:
    - **While Loop**:
    ```c
    int i = 0;
    while (i < 5) {
        printf("%d\n", i);
        i++;
    }
    ```

    - **For Loop**:
    ```c
    for (int i = 0; i < 5; i++) {
        printf("%d\n", i);
    }
    ```

- **Exit Controlled Loops**:
    - **Do-While Loop**:
    ```c
    int i = 0;
    do {
        printf("%d\n", i);
        i++;
    } while (i < 5);
    ```

### Nested Loops:
- **Example**: Multiplication Table
    ```c
    for (int i = 1; i <= 5; i++) {
        for (int j = 1; j <= 5; j++) {
            printf("%d\t", i * j);
        }
        printf("\n");
    }
    ```

### Jump Statements:
- **Break**:
    ```c
    for (int i = 0; i < 10; i++) {
        if (i == 5) {
            break;  // Exit loop when i equals 5
        }
        printf("%d\n", i);
    }
    ```

- **Continue**:
    ```c
    for (int i = 0; i < 5; i++) {
        if (i == 2) {
            continue;  // Skip the iteration when i equals 2
        }
        printf("%d\n", i);
    }
    ```

- **Goto**:
    ```c
    int i = 1;
    start:
    printf("%d\n", i);
    i++;
    if (i <= 5) {
        goto start;  // Jump back to label start
    }
    ```

- **Return**:
    ```c
    int sum(int a, int b) {
        return a + b;  // Return the sum of a and b
    }
    ```

## 2. Data Structures

### Arrays:
- **Example**: Array Declaration and Initialization
    ```c
    int arr[5] = {1, 2, 3, 4, 5};
    for (int i = 0; i < 5; i++) {
        printf("%d\n", arr[i]);
    }
    ```

- **Example**: Average of n Numbers Using Arrays
    ```c
    int marks[5], sum = 0;
    for (int i = 0; i < 5; i++) {
        scanf("%d", &marks[i]);
        sum += marks[i];
    }
    float average = sum / 5.0;
    printf("Average = %.2f\n", average);
    ```

### Strings:
- **Example**: String Declaration and Concatenation
    ```c
    char str1[20] = "Hello, ";
    char str2[20] = "World!";
    strcat(str1, str2);
    printf("%s\n", str1);  // Output: "Hello, World!"
    ```

## 3. Functions

### Standard Library Functions:
- **Example**: Using `printf()` and `scanf()`
    ```c
    int num;
    printf("Enter a number: ");
    scanf("%d", &num);
    printf("You entered: %d\n", num);
    ```

### User-Defined Functions:
- **Example**: Function with Arguments and Return Value
    ```c
    int add(int a, int b) {
        return a + b;
    }

    int main() {
        int result = add(3, 4);
        printf("Sum: %d\n", result);
        return 0;
    }
    ```

## 4. Parameter Passing

### Call by Value:
- **Example**: Swapping Two Numbers (Call by Value)
    ```c
    void swap(int x, int y) {
        int temp = x;
        x = y;
        y = temp;
        printf("Inside swap: x = %d, y = %d\n", x, y);
    }

    int main() {
        int a = 5, b = 10;
        swap(a, b);
        printf("Outside swap: a = %d, b = %d\n", a, b);
        return 0;
    }
    ```

### Call by Reference:
- **Example**: Swapping Two Numbers (Call by Reference)
    ```c
    void swap(int* x, int* y) {
        int temp = *x;
        *x = *y;
        *y = temp;
    }

    int main() {
        int a = 5, b = 10;
        swap(&a, &b);
        printf("After swap: a = %d, b = %d\n", a, b);
        return 0;
    }
    ```

## 5. Recursive Functions

- **Example**: Factorial Calculation (Recursive)
    ```c
    int factorial(int n) {
        if (n == 0) return 1;
        else return n * factorial(n - 1);
    }

    int main() {
        int num = 5;
        printf("Factorial of %d is %d\n", num, factorial(num));
        return 0;
    }
    ```

## 6. Macros

- **Example**: Defining Macros with and without Arguments
    ```c
    #define PI 3.14
    #define SQUARE(x) ((x) * (x))

    int main() {
        int radius = 5;
        printf("Area of circle: %.2f\n", PI * SQUARE(radius));
        return 0;
    }
    ```
