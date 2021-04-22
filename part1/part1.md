## Part 1a
1. 20
2. 20
3. 20
4. error, because the variable result declared by let is only visible in the if block, yet line 13 is outside of the if block,
so result is undeclared in that scope.
5. error, because result is declared constant and cannot be reassigned.
6. error, because the scope of variable declared by const is within the block. Line 13 is outside of the if block, so result is undeclared.

## Part 1b
1. 3 is printed. i is set to 3 after the last iteration of for loop. i is declared with var, so is visible at line 12.
2. 150 is printed. The discountedPrice is set to 300*0.5 = 150 after the last iteration of for loop. discountedPrice is declared with var, so is visible at line 13.
3. 150 is printed. The finalPrice is set to 150*100/100 = 150 after the last iteration of for loop. finalPrice is declared with var,
so is visible at line 13.
4. [50, 100, 150]. The discount is 0.5 so each of the price in the input is halved. discount is declared with var, so there's no problem with scope.
5. error: i is not defined. i is declared with let so is only visible in the for loop, but line 12 is outside of the loop.
6. error: discountedPrice is not defined. The variable is declared with let so is only visible in the for loop, but line 13 is outside of the loop.
7. 150. The value in the last iteration. Line 14 is in the same block as the let finalPrice declaration, so it is visible.
8. [50, 100, 150]. The discount is 0.5 so each of the price in the input is halved. The return statement is in the same block as the let discounted declaration, so it is visible.
9. error: i is not defined. is is declared with let in the for loop, but line 11 is outside of the loop.
10. 3. The const length declaration and line 12 are in the same block, so no problem iwth the scope. prices.length = 3.
11. [50, 100, 150]. There is no problem with the scope, and discounted is only mutated, not reassigned. No problem.

12. 
A. student.name
B. student['Grad Year']
C. student.greeting();
D. student['Favorite Teacher'].name
E. student.courseLoad[0];

13. 
A. 32. Integer 2 is mapped to '2'
B. 1. '3' is mapped to the integer 3
C. 0. null is mapped to 0
D. '3null'. null is mapped to 'null'
E. 4. true is mapped to 1
F. 0. false and null are mapped to 0.
G. '3undefined'. undefined is mapped to 'undefined'
H. NaN. Subtraction with non-numbers gives NaN

14. 
A. True. String is convert to a number in comparision.
B. False. Alphabetically 1 is less than 2
C. True. '2' is convert to 2
D. False. 2 and '2' are not the same time despite same value.
E. False. true is mapped to 1
F. True. Boolean(2) is true, same type and value as true

15. 
== checks for equality in value. === is the strict equality which checks both value and type.

17. 
[2, 4, 6]
The callback parameter of the modifyArray() is the function doSomething, which multiply its parameter by 2
each time it is called. In modifyArray([1,2,3], doSomething), we create a new array, walk through the parameter array,
and push the result of callback(array element) to the new array. So the result is [2, 4, 6].

19. 
1
4
3
2
The program will certainly execute line 2, 5 without setTimeout first. Then line 4 is time out immediately, and then line 3.