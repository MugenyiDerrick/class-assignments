this is the first submission about Writing program in C /C++ to find the maximum element in an array

#include <stdio.h>

int main() {
    int n, i, max;

    // Step 1: Input size of array
    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];  // declare array

    // Step 2: Input array elements
    printf("Enter %d numbers on the same line with spaces to separate them: ", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Step 3: Assume first element is max
    max = arr[0];

    // Step 4: Compare with other elements
    for(i = 1; i < n; i++) {
        if(arr[i] > max) {
            max = arr[i];
        }
    }

    // Step 5: Print result
    printf("Maximum element = %d\n", max);

    return 0;
}

