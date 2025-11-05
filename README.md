#include <stdio.h>

int main() {
    // ii. Declare and initialize our two score grids
    int scores1[2][2] = {
        {65, 92}, // Row 0
        {84, 72}  // Row 1
    };

    int scores2[2][2] = {
        {35, 70}, // Row 0
        {59, 67}  // Row 1
    };

    // iii. Print the first grid
    printf("Scores Grid 1:\n");
    // The outer loop handles each row
    for (int row = 0; row < 2; row++) {
        // The inner loop handles each column inside the current row
        for (int col = 0; col < 2; col++) {
            printf("%d ", scores1[row][col]); // Print the value
        }
        printf("\n"); // After a row is done, move to the next line
    }

    printf("\n"); // Add a blank line between the two grids

    // iii. Print the second grid
    printf("Scores Grid 2:\n");
    for (int row = 0; row < 2; row++) {
        for (int col = 0; col < 2; col++) {
            printf("%d ", scores2[row][col]);
        }
        printf("\n");
    }

    return 0;
}
