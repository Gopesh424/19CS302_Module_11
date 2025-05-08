## Task

# Write a function int max_of_four(int a, int b, int c, int d) which reads four arguments and returns the greatest of them.

## Note

There is not built in max function in C. Code that will be reused is often put in a separate function, e.g. int max(x, y) that returns the greater of the two values.

## Input Format

Input will contain four integers - a,b,c,d , one on each line.

## Output Format

Print the greatest of the four integers.
Note: I/O will be automatically handled.

## AIM:
  To determine a function int max_of_four(int a, int b, int c, int d) which reads four arguments and returns the greatest of them.

## ALGORITHM:
1. Start
2. Input four integers: a, b, c, and d
3. Call max(a, b) and store the result in a variable (e.g., max1)
4. Call max(c, d) and store the result in another variable (e.g., max2)
5. Call max(max1, max2) to get the greatest of all four values
6. Return the final result
7. End


## PROGRAM:
```
#include <stdio.h>

// Reusable function to return maximum of two integers
int max(int x, int y) {
    return (x > y) ? x : y;
}

// Function to return maximum of four integers using max()
int max_of_four(int a, int b, int c, int d) {
    return max(max(a, b), max(c, d));
}

int main() {
    int a, b, c, d;
    
    printf("Enter four integers: ");
    scanf("%d %d %d %d", &a, &b, &c, &d);

    int result = max_of_four(a, b, c, d);
    printf("Greatest value: %d\n", result);

    return 0;
}
```

## OUTPUT:
Enter four integers: 12 65 34 89

Greatest value: 89

## RESULT: 
Thus, the program is executed and verified successfully. 

