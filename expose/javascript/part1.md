**Var Declaration**<br>1. Line 9 will print 'values added: 20'<br>
2. Line 13 will print 'final result: 20'

**Let Declaration** <br>
3. Line 9 will print 'values added: 20' <br>
4. Line 13 will produce an error since the variable, result, was declared with a let keyword in the if statement, which means that 
the variable is accessible or visible within the if statement only. 

**Const Declaration**<br>
5. Line 9 will produce an error since the variable, result, was declared as a const variable which means that the variable
must be defined and assigned with a value and not cannot be reassigned afterwards. Here, the variable was be reassigned
to the sum of both parameters which causes the error. <br><br>
6. Line 13 will produce an error since not only was the const variable, result, reassigned to different value, it has the same scope as 
a let keyword so it is only visible within the if statement only and cannot be accessed outside. Here, the variable
was trying to be accessed outside the if statement which yields an error. 