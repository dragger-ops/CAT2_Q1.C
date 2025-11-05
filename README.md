#include <stdio.h>

int main() {
    // ii. Declare and initialize the arrays
    int scores1[2][2] = {
        {65, 92}, // Row 0
        {84, 72}  // Row 1
    };

    int scores2[2][2] = {
        {35, 70}, // Row 0
        {59, 67}  // Row 1
    };

    // iii. Print the first array
    printf("Elements of scores1:\n");
    for (int i = 0; i < 2; i++) {         // Outer loop: goes through each ROW
        for (int j = 0; j < 2; j++) {     // Inner loop: goes through each COLUMN in that row
            printf("%d ", scores1[i][j]); // Print the element at row 'i', column 'j'
        }
        printf("\n"); // After printing all columns in a row, go to the next line
    }

    // Print a newline to separate the two arrays
    printf("\n");

    // iii. Print the second array
    printf("Elements of scores2:\n");
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 2; j++) {
            printf("%d ", scores2[i][j]);
        }
        printf("\n");
    }

    return 0;
}
