# EX 55 C program to find a square of number using function with arguments without return type.
## DATE:08/05/2025
## AIM: To write a C program to find a square of number using function with arguments without return type.

## Algorithm
1. Start
2. Read an integer from the user and pass it as an argument to the square() function.
3. Inside the function, compute the square (num * num) and print the result.
4. End  


## Program:
```
#include <stdio.h>

// Function to compute square (no return, takes argument)
void square(int num) {
    int result = num * num;
    printf("Square of %d is %d\n", num, result);
}

int main() {
    int number;

    printf("Enter a number: ");
    scanf("%d", &number);

    // Function call with argument
    square(number);

    return 0;
}

/*
C program to find a square of number using function with arguments without return type.
Developed by: 
RegisterNumber:  
*/
```

## Output:
Enter a number: 7
Square of 7 is 49


## Result:
Thus the program was executed and the output was verified successfully.
