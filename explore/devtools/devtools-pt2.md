# DevTools - Debugging
1. The bug in the code is that the input data stored into num1 and num2 is by default, string. This means that
when the calculateSum() function computes the sum of these variables, it is actually concatenating the two
parameters causing the result to be string and not a sum of two numbers. 

2. To fix this bug, use type conversion to the input data where you use Number() on the value of the input. This
way num1 and num2 will be of number type and when calculateSum() is called, both variables will be added as numbers
which will be stored into result as a number type. 