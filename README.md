# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.
Seed the random number generator using the current time(i.e) rand(time(0));
Get the number of randon number to generate.
Pass the value for number of iterations and print the numbers.
End the program.

# PROGRAM:
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
    int n, i, start, end, randomNum;

    srand(time(0));

    printf("Enter the number of random numbers: ");
    scanf("%d", &n);

    printf("Enter the starting value: ");
    scanf("%d", &start);

    printf("Enter the ending value: ");
    scanf("%d", &end);

    if (start > end)
    {
        printf("Invalid range!\n");
        return 0;
    }

    printf("Random Numbers between %d and %d:\n", start, end);

    for(i = 0; i < n; i++)
    {
        randomNum = start + rand() % (end - start + 1);
        printf("%d\n", randomNum);
    }

    return 0;
}
```
# OUTPUT:
<img width="408" height="482" alt="Screenshot 2026-07-31 091301" src="https://github.com/user-attachments/assets/df06d307-c035-4059-8785-9bc32b61ef09" />




















# RESULT:
The program is executed successfully
