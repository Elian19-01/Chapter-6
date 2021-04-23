# Chapter-6
Solve the the exercises from chapter 6 of "Practical C programming" 

### Exercise 6-1: Write a program to find the square of the distance between two
points. (For a more advanced problem, find the actual distance. This problem
involves u sing the standard function sqrt. Use your help system to find out more
about how to use this function.)

```c
#include <stdio.h>
#include <math.h>

int main() {
	float x1, y1, x2, y2, gdistance;
	printf("Input x1: ");
	scanf("%f", &x1);
	printf("Input y1: ");
	scanf("%f", &y1);
              printf("Input x2: ");
	scanf("%f", &x2);
	printf("Input y2: ");
	scanf("%f", &y2);
	gdistance = ((x2-x1)*(x2-x1))+((y2-y1)*(y2-y1));
	printf("Distance between two points are: %.4f", sqrt(gdistance));

	return 0;
}
```
### Exercise 6-4: Given an amount of money (less than $1.00), compute the number
of quarters, dimes, nickels, and pennies needed.


```c
#include <stdio.h>

char line[100];             
int cents;                  
int quarters         
int dimes            
int nickels        
int pennies          

int main() {
	printf("Enter the number of cents we have: ");
	fgets(line, sizeof(line), stdin);
	sscanf(line, "%d", &cents);

	if (cents > 99) {
		printf("You haven't enogh money\n");
		return(1);
	} else if (cents < 1) {
		printf("Error: can not be less than a penny\n");
		return(1);
	}

	while  {
		if (cents >= 25) {
			++quarters;
			cents -= 25;
		} else if (cents >= 10) {
			++dimes;
			cents -= 10;
		} else if (cents >= 5) {
			++nickels;
			cents -= 5;
		} else if (cents >= 1) {
			++pennies;
			--cents;
		} else if (cents = 0) {

		}
	}

	printf("%d quarters %d dimes %d nickels %d pennies\n",
		quarters, dimes, nickels, pennies);

	return(0);
}


```
###Exercise 6-5: A leap year is any year divisible by 4, unless the year is divisible by
100, but not 400. Write a program to tell if a year is a leap year.


```c
#include <stdio.h>
int main() {
   int year;
   printf("Enter a year: ");
   scanf("%d", &year);

  
   if (year % 400 == 0) {
      printf("%d is a leap year.", year);
   }
   else if (year % 100 == 0) {
      printf("%d is not a leap year.", year);
   }
   
   else if (year % 4 == 0) {
      printf("%d is a leap year.", year);
   }
  
   return 0;
}

```



