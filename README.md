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
