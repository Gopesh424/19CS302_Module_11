# EX 53 C program to remove duplicates in an array.
## DATE:
## AIM:
To write a C program to remove duplicates in an array.

## Algorithm
1. Start
2. Iterate through the input array, and for each element, check if it already exists in the result array.
3. If it doesn't exist in result, add it to the result array.
4. Return the size of the result array with duplicates removed.
5. End 

## Program:
```
#include <stdio.h>

// Function to remove duplicates
int removeDuplicates(int arr[], int n, int result[]) {
    int i, j, k = 0;
    int isDuplicate;

    for (i = 0; i < n; i++) {
        isDuplicate = 0;

        // Check if arr[i] is already in result[]
        for (j = 0; j < k; j++) {
            if (arr[i] == result[j]) {
                isDuplicate = 1;
                break;
            }
        }

        // If not duplicate, add to result[]
        if (!isDuplicate) {
            result[k] = arr[i];
            k++;
        }
    }

    return k; // Return the size of result[]
}

int main() {
    int arr[] = {4, 5, 9, 4, 9, 6, 7, 5};
    int n = sizeof(arr) / sizeof(arr[0]);
    int result[100]; // Assuming max 100 elements
    int i;

    int newSize = removeDuplicates(arr, n, result);

    printf("Array after removing duplicates: ");
    for (i = 0; i < newSize; i++) {
        printf("%d ", result[i]);
    }
    printf("\n");

    return 0;
}

/*
C program to remove duplicates in an array
Developed by: 
RegisterNumber:  
*/
```

## Output:
Array after removing duplicates: 4 5 9 6 7


## Result:
Thus the program was executed and the output was verified successfully.
