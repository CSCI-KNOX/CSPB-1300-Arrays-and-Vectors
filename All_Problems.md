## Problem: Find Smallest

Write a function, double smallest(double x, double y, double z), that returns the value of the smallest of its three input parameters. 

#### Hint:
If the first number is less than or equal to both of the other two numbers, then the first number is considered the smallest
Else if the second number is less than or equal to both of the other two numbers, then the second number is considered the smallest
Else the third number is considered the smallest


#### Function prototype:
	/**
	   Returns the smallest of the three parameters.
	   @param x the first number
	   @param y the second number
	   @param z the third number
	   @return a double which is the smallest of the three params
	*/


	double smallest(double x, double y, double z);
#### Note: 
You may assume that the iostream, fstream, string, cmath, vector, and algorithm standard headers and the "using namespace std" directive are already included.

#### Test Cases:
	
| Test	| Result |
|--- | --- |
| cout << smallest(2.5, 10, 3.3); | 2.5 |
| cout << smallest(13.33, 1.7, 200); | 1.7 |
	


_______________________________

## Problem: Check if all values are different
Write a function, bool all_different(double x, double y, double z), that returns true if the three input parameters are all different (i.e., not equal) or false otherwise.

#### Hint: 
If the first number doesn't equal the second number, the second number doesn't equal the third number, and the first number doesn't equal the third number, then they are considered all different.

#### Function prototype:
	/**
	   Determines if the three parameters are all NOT equal.
	   @param x the first number
	   @param y the second number
	   @param z the third number
	   @return true if all different, otherwise false
	*/
	bool all_different(double x, double y, double z);

#### Note: 
You may assume that the iostream, fstream, string, cmath, vector, and algorithm standard headers and the "using namespace std" directive are already included.

#### Test Cases:

<!-- 
<table align="left">
<thead>
<tr>
<th>Test</th>
<th>Results</th>
</tr>
</thead>
<tbody>
<tr>
<td>cout << all_different(2.1, 2.1, 3.2);</td>
<td>0</td>
<tr>
<td>cout << all_different(3.5, 12.7, 6);</td>
<td>1</td>
</tr>
</tbody>
</table>
 -->

| Test	| Result |
|--- | --- |
| cout << all_different(2.1, 2.1, 3.2); | 0 |
| cout << all_different(3.5, 12.7, 6); | 1 |

_______________________________

## Problem: Repeat given string

Write a function, string repeat(string str, int n), that returns the string str repeated n times. For example, repeat("ho", 3) returns "hohoho".

#### Hint:
Create a new string
Using the accumulation pattern, iterate the number of times specified by the input number and concatenate the input string to the new string on each iteration

#### Function prototype:
	/**
	   Repeats a given word multiple times.
	   @param str a string with initial word
	   @param n the number of times to repeat
	   @return a string with the repeated word
	*/
	string repeat(string str, int n);

#### Note: 
You may assume that the iostream, fstream, string, cmath, vector, and algorithm standard headers and the "using namespace std" directive are already included.

#### Test Cases:

| Test | Result |
| :-- | :-- |
| cout << repeat("hi", 3); | hihihi|
| cout << repeat("bye", 5); | byebyebyebyebye |



_______________________________

## Problem: Swap Values

Write a function, void sort2(int& a, int& b), that swaps the values of a and b if a is greater than b and otherwise leaves a and b unchanged. For example:
	int u = 2;
	int v = 3;
	sort2(u, v); // u is still 2 and v is still 3 after this function call

	int w = 4;
	int x = 1;
	sort2(w, x); // w is now 1 and x is now 4 after this function call
	
#### Hint:
Note that the parameters are reference parameters so you should be updating their values directly in your function (you don't return anything from this function)
If you want to swap the values in two variables:
Copy the value of the first variable into a new temporary variable
Update the first variable with the value of the second variable
Now update the second variable with the value of the temporary variable

#### Function prototypes:
	/**
	   Swaps values of the parameters provided the first parameter
	   is larger than the second.
	   @param a first input value
	   @param b second input value
	   @return nothing
	*/
	void sort2(int& a, int& b);
#### Note: 
You may assume that the iostream, fstream, string, cmath, vector, and algorithm standard headers and the "using namespace std" directive are already included.

#### Test Cases:


<table align="left">
<thead>
<tr>
<th>Test</th>
<th>Results</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<br>	int u = 2;
<br>	int v = 3;
<br>	sort2(u, v);
<br>	cout << u << endl;
<br>	cout << v;
</td>
<td>2<br>3</td>
<tr>
<td>
<br>	int w = 4;
<br>	int x = 1;
<br>	sort2(w, x);
<br>	cout << w << endl;
<br>	cout << x;
</td>
<td>1<br>4</td>
</tr>
</tbody>
</table>