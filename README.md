#include <stdio.h>

void generateOddSeries(int x) {
    int i;
    for (i = 1; i <= x; i++) {
        if (i % 2 != 0) {
            printf("%d", i);
            if (i < x) {
                printf(", ");
            }
        }
    }
    printf("\n");
}

int main() {
    int x;

    printf("Enter a number (x): ");
    scanf("%d", &x);

    printf("Output: ");
    generateOddSeries(x);

    return 0;
}
