1. At line 12, the value of the global variable i will be printed out, which is 3. This variable
is a counter variable and increments until it reaches end of array. This was able to 
be printed because i was declared with a var keyword, meaning it has no block scope
and can be even accessed even after the for loop ends. 

2. At line 13, the value of the global variable discountedPrice will be printed out, which
is 150 since the last value to be stored into this variable uses the last element of the 
array, 300, multiplied with (1 - 0.5) which yields to 150. Just like i, this variable has
no block scope and can be accessed after the for loop ends.

3. At line 14, the value of the global variable finalPrice will be printed, which is 150.
The last value to be stored into this variable utilizes the last variable stored in 
discountedPrice and multiplies it with 100, rounds this value and divides by 100. 
Just like the 2 other variables, finalPrice can be accessed outside the for loop
after done executing.

4. The function will return an array of the discounted prices computed in the for loop.
The array, discounted, will contain: [50, 100, 150]. Every value from the original
array is modified using the discount and pushed into the new array.

5. At line 12, an error will be produced since i was declared with a let keyword, meaning
it can only be visible and accessed in the for loop only and nowhere else. 

6. At line 13, an error will be produced since discountedPrice was declared with a let keyword, meaning
it also can be accessed in the for loop only and nowhere else.

7. At line 14, the value of finalPrice will be printed out which is 150. Although declared with a 
let keyword, this variable is accessible throughout the whole function including inside the for loop
since it has a larger scope than i and discountedPrice.

8. The function will return an array of the discounted prices computed in the for loop.
The array, discounted, will contain: [50, 100, 150]. Regardless of being declared as let or 
var, the array is accessible throughout the function so it was able to add the discounted values
into it.

9. At line 11, an error will be produced since i was declared with a let keyword, meaning
it can only be visible and accessed in the for loop only and nowhere else. 

10. At line 12, the value of length will be printed, which is 3. Although marked with a const keyword,
the variable has not been reassigned, it's value is just printed out. 

11. The function will return an array of the discounted prices computed in the for loop.
The array, discounted, will contain: [50, 100, 150]. Even though it was marked with a const keyword, 
this only refers to the reference of the array, not the contents. This means that if discounted
was explicitly assigned to another array, then it points to another array and changes its reference,
which then would cause an error. However, adding elements to it does not change the actual reference
of the array, discounted.