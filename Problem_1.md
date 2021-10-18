## Problem 1

Write a function, double smallest(double x, double y, double z), that returns the value of the smallest of its three input parameters. 

### Hint:
If the first number is less than or equal to both of the other two numbers, then the first number is considered the smallest
Else if the second number is less than or equal to both of the other two numbers, then the second number is considered the smallest
Else the third number is considered the smallest


	Function prototype:
	/**
	   Returns the smallest of the three parameters.
	   @param x the first number
	   @param y the second number
	   @param z the third number
	   @return a double which is the smallest of the three params
	*/


	double smallest(double x, double y, double z);
### Note: 
You may assume that the iostream, fstream, string, cmath, vector, and algorithm standard headers and the "using namespace std" directive are already included.

### For example:

| Test	| Result|
|-------||
|cout << smallest(2.5, 10, 3.3); | 2.5 |
| cout << smallest(13.33, 1.7, 200); | 1.7 |
