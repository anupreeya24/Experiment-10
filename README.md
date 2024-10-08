# Experiment-10

# Experiment-10
**Aim:** <br>
To study and implement Pointer Operations (call by value and call by reference) <br>
<br>
**Theory:** <br>
There are two ways to call a variable to a function for various operations. <br>
| Call by Value  | Call by Reference |
| ------------- | ------------- |
| A method of passing arguments to a function where the actual value is passed.  | A method of passing arguments where the address of the variable is passed.  |
| Does not affect the original variable.  | Does affect the original variable.  |
| More memory is used because a copy of the actual value is made.  | Less memory is used because only the address is passed.  |
| Used when the function does not need to modify the original data.  | Used when the function needs to modify the original data or when passing large objects.  |
<br>



### Algorithm to Swap Two Integers

1. **Define Swap Function**:
   - Create a function `swap(int x, int y)` that takes two integers as parameters.
   - Inside the function:
     - Declare a temporary integer `temp`.
     - Assign the value of `x` to `temp`.
     - Assign the value of `y` to `x`.
     - Assign the value of `temp` to `y`.
   

2. **Main Function**:
   - Initialize two integers `a` and `b` with values (e.g., `5` and `2`).
   - Call the `swap` function with `a` and `b` as arguments.

3. **Display Values**:
   - Print the values of `a` and `b` after the swap function is called.


### Algorithm to Swap Two Integers Using Pointers

1. **Define Swap Function**:
   - Create a function `swap(int *x, int *y)` that takes two integer pointers as parameters.
   - Inside the function:
     - Declare a temporary integer `temp`.
     - Assign the value pointed to by `x` to `temp` (`temp = *x`).
     - Assign the value pointed to by `y` to the location pointed to by `x` (`*x = *y`).
     - Assign the value in `temp` to the location pointed to by `y` (`*y = temp`).

2. **Main Function**:
   - Initialize two integers `a` and `b` with values (e.g., `5` and `2`).
   - Call the `swap` function with the addresses of `a` and `b` (`swap(&a, &b)`).

3. **Display Values**:
   - Print the values of `a` and `b` after the swap function is called.
