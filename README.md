# EX-NO-6-Pseudo-Random-Number

## AIM : 
To implement Pseudorandom Number Generation using Standard library

## ALGORITHM : 
```
Step 1: Get the number of random numbers to generate from the user.
Step 2: Read the minimum and maximum values for the random number range.
Step 3: Initialize the random seed using the current time.
Step 4: Generate a random number by calculating the remainder of division with the range
(max - min + 1) and adding the minimum value.
Step 5: Repeat the random number generation for the specified count.
Step 6: Print each generated random number.
Step 7: End the program.
```
## PROGRAM : 
### NAME: HAARISH V
### REGISTER NO: 212223230067
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
int count, min, max;

printf("Enter the number of random numbers to generate: ");
scanf("%d", &count);
printf("Enter the minimum value: ");
scanf("%d", &min);
printf("Enter the maximum value: ");
scanf("%d", &max);
srand(time(NULL));
printf("Pseudorandom numbers:\n");

for (int i = 0; i < count; i++)
{
int random_number = (rand() % (max - min + 1)) + min;
printf("%d\n", random_number);
}
return 0;
}
```
## OUTPUT : 
![Screenshot 2025-04-07 223345](https://github.com/user-attachments/assets/252ca0d3-47c8-4bd5-ab52-1c86a6d68d2f)
## RESULT:
Thus Pseudorandom Number Generation using Standard library is implemented successfully.

