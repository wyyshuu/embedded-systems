c in es
//grading system
include <stdio.h>

int main() {
    int number;

    printf("Enter a number: ");
    scanf("%d", &number);

    if (number < 0) {
        if (number % 5 == 0) {
            printf("The number is negative and divisible by 5.\n");
        } else {
            printf("The number is negative but not divisible by 5.\n");
        }
    } else if (number == 0) {
        printf("The number is zero.\n");
    } else {
        if (number % 2 == 0) {
            printf("The number is even.\n");
        } else {
            printf("The number is odd.\n");
        }
    }

    return 0;
}
//discount
#include <stdio.h>

int main() {
    int age;

    // Prompting user to enter age
    printf("Enter age: ");
    scanf("%d", &age);

    // Checking discount conditions
    if (age < 12)
        printf("You get 50%% discount\n");
    else if (age == 18)
        printf("You get 20%% discount\n");
    else if (age >= 60)
        printf("You get 30%% discount\n");
    else
        printf("You get 10%% discount\n");

    return 0;
}
    
//even and odd
   #include <stdio.h>

int main() {
    int range;

    printf("Enter your range (1-4): ");
    scanf("%d", &range);

    switch (range) {
        case 1:
            printf("90-100\n");
            break;
        case 2:
            printf("80-89\n");
            break;
        case 3:
            printf("70-79\n");
            break;
        case 4:
            printf("Below 70\n");
            break;
        default:
            printf("Error: Invalid range!\n");
            break;
    }

    return 0;
}
//shapes
#include <stdio.h>

int main() {
    int choice;
    float side, length, width, base, height;

    printf("Shape Area Calculator\n");
    printf("1. Square\n");
    printf("2. Rectangle\n");
    printf("3. Triangle\n");
    printf("Enter your choice (1-3): ");
    scanf("%d", &choice);

    if (choice == 1) {
        printf("Enter side length: ");
        scanf("%f", &side);
        printf("Area: %.2f\n", side * side);
    } else if (choice == 2) {
        printf("Enter length and width: ");
        scanf("%f %f", &length, &width);
        printf("Area: %.2f\n", length * width);
    } else if (choice == 3) {
        printf("Enter base and height: ");
        scanf("%f %f", &base, &height);
        printf("Area: %.2f\n", 0.5 * base * height);
    } else {
        printf("Invalid choice\n");
    }

    return 0;
}


