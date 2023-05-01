# Part 2
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

12. 
    **A.** student.name or student['name'] <br>
    **B.** student['Grad Year'] <br>
    **C.** student.greeting() <br>
    **D.** student['Favorite Teacher'].name or student['Favorite Teacher']['name']<br>
    **E.** student.courseLoad[0] or student['courseLoad'][0]

13. 
    **A.** '32'; Javascript changes 2 to be a string so that the concatenation can be made, resulting in '32.' <br>
    **B.** 1; '3' is converted to a number 3, which then is subtracted by 2 to get 1.<br>
    **C.** 3; null is converted to 0, so 3 can be added to 0 to get 3.<br>
    **D.**'3null'; null was converted to a string 'null' allowing for concatenation to result in '3null' <br>
    **E.** 4; true was converted to its number counterpart, 1, which was added to 3 yielding 4.<br>
    **F.** 0; both false and null were converted to the number 0 so adding both 0's led to 0.<br>
    **G.** '3undefined'; undefined was converted to the string 'undefined' resulting in a string concatenation of '3undefined.'<br>
    **H.** NaN; undefined was converted trying to be converted to a number in order to carry out the subtraction operation. However,
    the numerical equivalence of undefined is NaN, which makes the overall output to be NaN. <br>

14. 
    **A.** true; '2' becomes the number 2 which is greater than 1, thus the result is true. <br>
    **B.** false; both '2' and '12' are converted to the numbers 2 and 12, and 2 is not less than 12, which leads to false. <br>
    **C.** true; '2' is converted to number 2 which is equal to 2, leading to the result to be true. <br>
    **D.** false; both 2 and '2' are different data types, so the answer is false. <br>
    **E.** false; true is converted to number 1 which is not equal to 2, so the result is false. <br>
    **F.** true; both true and Boolean(2) are of the same data type and the values are the same, so the overall result is true. <br>

15. The "==" opeartor aims to convert data types by default, if different data types are compared and checks if the values are equal or not. 
However, "===" is known as the strict equality operator which means that if different data types are compared using this operator, then 
the output will always be false without any conversion. It may be true if the data types are the same and have the same values, otherwise false
if values are different even if same data type. 

16. **In Corresponding JS File**

17. The modifyArray function will return the array: [2, 4, 6]. The function creates a new array and traverses through
the array parameter. In each iteration the callback function, doSomething, is called and returns the number argument times 2. 
This value is then pushed into the array. After the loop ends, the new array is returned at the end. <br>

18. **In Corresponding JS File**

19. This function prints out 1 and 4 immediately. Then it will go to the setTimeout functions where it will print 3 immediately since
the timer was 0 milliseconds, and then the function waits for 1000 milliseconds or 1 second to print out 2. 