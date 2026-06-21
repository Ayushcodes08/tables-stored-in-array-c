# Multiplication Table Generator in C

This is a simple C program that demonstrates the use of **2D arrays**, **nested loops**, and **array indexing**.

## Description

The program creates multiplication tables for the numbers:

- 2
- 7
- 9

The tables are stored in a 2D array and then displayed on the screen.

## How It Works

1. A 2D array `arr[3][10]` is created.
2. An array `mul[] = {2, 7, 9}` stores the numbers whose tables will be generated.
3. Nested loops fill the 2D array with multiplication values.
4. Another set of nested loops prints all the values.

## Example Output

```
The value of arr[0][0] is 2
The value of arr[0][1] is 4
The value of arr[0][2] is 6
...
The value of arr[1][0] is 7
The value of arr[1][1] is 14
...
The value of arr[2][9] is 90
```

## Concepts Used

- C Programming
- Arrays
- 2D Arrays
- Nested Loops
- Array Traversal

## Source Code

```c
#include <stdio.h>

int main() {
    int arr[3][10];
    int mul[] = {2, 7, 9};

    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 10; j++) {
            arr[i][j] = mul[i] * (j + 1);
        }
    }

    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 10; j++) {
            printf("The value of arr[%d][%d] is %d\n", i, j, arr[i][j]);
        }
    }

    return 0;
}
```

## Author

Ayush Ojha

## License

This project is open-source and available for learning purposes.
