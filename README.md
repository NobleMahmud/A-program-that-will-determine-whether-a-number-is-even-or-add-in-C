# A-program-that-will-determine-whether-a-number-is-even-or-add-in-C

#include <stdio.h>

char* checkEvenOdd(int number) {
    if (number % 2 == 0) {
        return "Even";
    } else {
        return "Odd";
    }
}

int main() {
    int num;
    printf("Enter a number: ");
    scanf("%d", &num);

    char* result = checkEvenOdd(num);
    printf("The number %d is %s.\n", num, result);

    return 0;
}



# A program that will determine whether a number is positive or negative in C

#include <stdio.h>

void checkPositiveNegative(int number) {
    if (number > 0) {
        printf("The number is positive.\n");
    } else if (number < 0) {
        printf("The number is negative.\n");
    } else {
        printf("The number is zero.\n");
    }
}

int main() {
    int num;
    printf("Enter a number: ");
    scanf("%d", &num);

    checkPositiveNegative(num);

    return 0;
    
   
   
# A program that will determine the first n Fibonacci numbers in C 
    #include <stdio.h>

void printFibonacciNumbers(int n) {
    int first = 0, second = 1, next, i;

    printf("The first %d Fibonacci numbers are:\n", n);

    for (i = 0; i < n; i++) {
        if (i <= 1) {
            next = i;
        } else {
            next = first + second;
            first = second;
            second = next;
        }
        printf("%d ", next);
    }
    printf("\n");
}

int main() {
    int n;
    printf("Enter the value of n: ");
    scanf("%d", &n);

    printFibonacciNumbers(n);

    return 0;
}


# The moon’s gravity is about 17 percent of Earth’s. Write a
program that allows you to enter your weight and computes
your effective weight on the moon. Write a code in C.

#include <stdio.h>

int main() {
    float weightEarth, weightMoon;

    printf("Enter your weight on Earth (in kg): ");
    scanf("%f", &weightEarth);

    weightMoon = weightEarth * 0.17;

    printf("Your weight on the Moon would be: %.2f kg\n", weightMoon);

    return 0;
}



# Factorial program in c: c code to find and print factorial of a
number, three methods are given, first one uses for loop,
second uses a function to find factorial and third using
recursion. Factorial is represented using'!', so five factorial
will be written as(5!), n factorial as (n!).Also
n!=n*(n-1)*(n-2)*(n-3)...3.2.1 and zero factorial is defined as
onei.e.0!=1.

unsigned long long factorialRecursion(int n) {
    if (n == 0) {
        return 1;
    } else {
        return n * factorialRecursion(n - 1);
    }
}

int main() {
    int num;
    printf("Enter a number: ");
    scanf("%d", &num);
    
    
    
