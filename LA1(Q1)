#include <stdio.h>

// Function to calculate factorial
long long factorial(int n) {
    long long fact = 1;
    for (int i = 1; i <= n; i++) {
        fact = fact * i;
    }
    return fact;
}

int main() {
    int n, r, choice;
    long long result;

    printf("---- Permutation and Combination Calculator ----\n");
    printf("1. Permutation (nPr)\n");
    printf("2. Combination (nCr)\n");
    printf("Enter your choice (1 or 2): ");
    scanf("%d", &choice);

    printf("Enter value of n: ");
    scanf("%d", &n);

    printf("Enter value of r: ");
    scanf("%d", &r);

    // Input validation
    if (n < 0 || r < 0 || r > n) {
        printf("Invalid input! Ensure that n >= r and both are non-negative.\n");
        return 0;
    }

    if (choice == 1) {
        // nPr = n! / (n-r)!
        result = factorial(n) / factorial(n - r);
        printf("Permutation (nPr) = %lld\n", result);
    }
    else if (choice == 2) {
        // nCr = n! / (r! * (n-r)!)
        result = factorial(n) / (factorial(r) * factorial(n - r));
        printf("Combination (nCr) = %lld\n", result);
    }
    else {
        printf("Invalid choice!\n");
    }

    return 0;
}
