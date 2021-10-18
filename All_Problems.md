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
<pre>
	int u = 2;
	int v = 3;
	sort2(u, v); // u is still 2 and v is still 3 after this function call

	int w = 4;
	int x = 1;
	sort2(w, x); // w is now 1 and x is now 4 after this function call
</pre>

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

<table>
<thead><tr><th>Test</th><th>Results</th></tr></thead>
<tbody>
<tr><td><pre>
int u = 2;
int v = 3;
sort2(u, v);
cout << u << endl;
cout << v;
</pre></td>
<td><pre>
2
3



</pre></td>
<tr><td><pre>
int w = 4;
int x = 1;
sort2(w, x);
cout << w << endl;
cout << x;
</pre></td>
<td><pre>
1
4


</pre></td>
</tr>
</tbody>
</table>

_______________________________


## Problem: Swap first with last
Write a function that swaps the first and last element in an array of integers.

#### Hint: 
Review 6.2.10 on Swapping Elements in the Big C++ book.

#### Function prototype:
	/**
	   swaps first and last elements of int array
	   @param arr[]  the array
	   @param size number of elements
	   @return nothing
	*/
	void swap_first_last(int arr[], int size);
#### Note: 
You may assume that the iostream, fstream, string, cmath, vector, and algorithm standard headers and the "using namespace std" directive are already included.

#### Test Cases:

<table>
<thead><tr><th>Test</th><th>Results</th></tr></thead>
<tbody>
<tr><td><pre>
int values[] = {1, 2, 3, 4, 5};
int size = 5;
swap_first_last(values, size);
for (int i = 0; i < size; i++) {
	cout << values[i] << " ";
}
</pre></td>
<td>5 2 3 4 1</td>
<tr><td><pre>
int values[] = {5, 8, 1, 74, 2, 13, 12};
int size = 7;
swap_first_last(values, size);
for (int i = 0; i < size; i++) {
   cout << values[i] << " ";
}
</pre></td>
<td>12 8 1 74 2 13 5</td>
</tr>
</tbody>
</table>

_______________________________


## Problem: Replace elements within an array
Write a function that replaces all even elements with 0 in an array of integers.

#### Hint:
Iterate through the elements of the input array
If the element is even, then update the value of the element to 0

#### Function prototype:
	/**
	   Replace even elements of int array with zero
	   @param arr[]  the array
	   @param size number of elements
	   @return nothing
	*/
	void replace_even(int arr[], int size);
	
#### Note: 
You may assume that the iostream, fstream, string, cmath, vector, and algorithm standard headers and the "using namespace std" directive are already included.


#### Test Cases:

<table>
<thead><tr><th>Test</th><th>Results</th></tr></thead>
<tbody>
<tr><td><pre>
int values[] = {1, 4, 9, 16, 25};
int size = 5;
replace_even(values, size);
for (int i = 0; i < size; i++) {
   cout << values[i] << " ";
}
</pre></td>
<td><pre>
1 0 9 0 25



</pre></td>
<tr><td><pre>
int values[] = {5, 8, 1, 74, 2, 13, 12};
int size = 7;
replace_even(values, size);
for (int i = 0; i < size; i++) {
   cout << values[i] << " ";
}
</pre></td>
<td><pre>
5 0 1 0 0 13 0




</pre></td>
</tr>
</tbody>
</table>

_______________________________

## Problem: Remove Minimum Value
Write a function that removes the minimum value from a partially filled array without calling other functions. You must also update the size reference parameter.

#### Hint:
First, find the minimum value in the array, but remember to also save the index of that minimum value
Refer to 6.2.4 on Maximum and Minimum in the Big C++ book
Then, remove that minimum value using the index you saved
Refer to 6.2.8 on Removing an Element from an Ordered Array
Don't forget to update the size reference parameter

#### Function prototype:
<pre>
/**
   Removes the minimum value.
   @param input[] the array
   @param size number of elements
   @return nothing
*/
void remove_min(double input[], int &size);
</pre>

#### Note: 
You may assume that the iostream, fstream, string, cmath, vector, and algorithm standard headers and the "using namespace std" directive are already included.

#### Test Cases:

<table>
<thead><tr><th>Test</th><th>Results</th></tr></thead>
<tbody>
<tr><td><pre>
double values[] = {9.1, 2.5, 3, 30.8, 25};
int size = 5;
remove_min(values, size);
for (int i = 0; i < size; i++) {
   cout << values[i] << " ";
}
</pre></td>
<td><pre>
9.1 3 30.8 25




</pre></td>
<tr><td><pre>
double values[] = {5.9, 8, 1.1, 74, 2.7, 13};
int size = 6;
remove_min(values, size);
for (int i = 0; i < size; i++) {
   cout << values[i] << " ";
}
</pre></td>
<td><pre>
5.9 8 74 2.7 13




</pre></td>
</tr>
</tbody>
</table>

_______________________________

## Problem: 

#### Test Cases:

<table>
<thead><tr><th>Test</th><th>Results</th></tr></thead>
<tbody>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
</tr>
</tbody>
</table>
_______________________________

## Problem: 

#### Test Cases:

<table>
<thead><tr><th>Test</th><th>Results</th></tr></thead>
<tbody>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
</tr>
</tbody>
</table>
_______________________________

## Problem: 

#### Test Cases:

<table>
<thead><tr><th>Test</th><th>Results</th></tr></thead>
<tbody>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
</tr>
</tbody>
</table>
_______________________________

## Problem: 

#### Test Cases:

<table>
<thead><tr><th>Test</th><th>Results</th></tr></thead>
<tbody>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
</tr>
</tbody>
</table>
_______________________________

## Problem: 

#### Test Cases:

<table>
<thead><tr><th>Test</th><th>Results</th></tr></thead>
<tbody>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
</tr>
</tbody>
</table>
_______________________________

## Problem: 

#### Test Cases:

<table>
<thead><tr><th>Test</th><th>Results</th></tr></thead>
<tbody>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
</tr>
</tbody>
</table>
_______________________________

## Problem: 

#### Test Cases:

<table>
<thead><tr><th>Test</th><th>Results</th></tr></thead>
<tbody>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
<tr><td><pre>
code
</pre></td>
<td><pre>
result
</pre></td>
</tr>
</tbody>
</table>