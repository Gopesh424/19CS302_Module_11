## print all the letters of the English alphabet.

SAMPLE OUTPUT : CAPS and add space to each alphabet

A B C D E F G H I J K L M N O P Q R S T U V W X Y Z

## AIM:
 To print all the letters of the English alphabet.

## ALGORITHM:
1. Start
2. Loop from character 'A' to 'Z', and in each iteration:
3. Print the character followed by a space.
4. End the loop and print a newline


## PROGRAM:
```
#include <stdio.h>

int main() {
    char ch;

    printf("Output:\n");

    for (ch = 'A'; ch <= 'Z'; ch++) {
        printf("%c ", ch);
    }

    printf("\n");
    return 0;
}
```

## OUTPUT:
Output:

A B C D E F G H I J K L M N O P Q R S T U V W X Y Z


## RESULT:

Thus, the program is executed and verified successfully.



















