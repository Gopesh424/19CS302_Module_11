# EX 51 C program to reverse a string.
## DATE:08/05/2025
## AIM: To write a C program to reverse a string.

## Algorithm
1. Start
2. Input the string from the user.
3. Initialize two pointers: start at 0, and end at the last character of the string.
4. Swap the characters at start and end.
5. Move start forward and end backward.
6. Repeat steps 3–4 until start >= end.
7. End


## Program:
```
#include <stdio.h>
#include <string.h>

// Function to reverse a string
void reverseString(char str[]) {
    int start = 0;
    int end = strlen(str) - 1;
    char temp;

    while (start < end) {
        // Swap characters
        temp = str[start];
        str[start] = str[end];
        str[end] = temp;

        // Move towards the center
        start++;
        end--;
    }
}

int main() {
    char str[100];

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    // Remove newline character if present
    size_t len = strlen(str);
    if (len > 0 && str[len - 1] == '\n') {
        str[len - 1] = '\0';
    }

    reverseString(str);

    printf("Reversed string: %s\n", str);
    return 0;
}

/*
C program to reverse a string.
Developed by: 
RegisterNumber:  
*/
```

## Output:
Enter a string: hello world

Reversed string: dlrow olleh


## Result:
Thus the program was executed and the output was verified successfully.
