1. the length of the prices array will be printed, because var has no block scope
2. the discountedPrice that corresponds to the last element of the prices array will be printed, because var has no block scope. Although discountedPrice is declared in the for loop block, it will still be printed
3. the finalPrice that corresponds to the last element of the prices array will be printed, because the value of var is modified in the for loop and var has no block scope.
4. [50, 100, 150], because var has no block scope, therefore they can be accessed and modified no matter where they are declared (inside the for loop or not). Therefore the function will work as intended which multiplies the elements of the array by (1 - discount) and round to integer by using the for loop, which gives the result [50, 100, 150]
5. A variable not defined error will be printed, because when declare variables using let inside a block, that variable is only visibile inside that block. Therefore, since i is declared in the for loop, it will not be visible to anymore once the loop ends.
6. A variable not defined error will be printed, because when declare variables using let inside a block, that variable is only visibile inside that block. Therefore, since discountedPrice is declared in the for loop, it will not be visible anymore once the loop ends.
7. the finalPrice that corresponds to the last element of the prices array will be printed, because finalPrice is declared in the same block as the console.log statement (within the function block) and therefore can be accessed by the for loop and the console.log statement.
8. [50, 100, 150], Assuming line 11, 12 and 13 somehow doesn't throw any errors, then the function will work as intended, because the discounted array is declared in the same block as the return statement (within the function block). Therefore the function will work as intended which multiplies the elements of the array by (1 - discount) and round to integer by using the for loop, which gives the result [50, 100, 150]
9. A variable not defined error will be printed, because when declare variables using let inside a block, that variable is only visibile inside that block. Therefore, since i is declared in the for loop, it will not be visible to anymore once the loop ends.
10. Disregarding the error in previous lines that const can't be reassigned, a variable not defined error will be printed, because when declare variables using const inside a block, that variable is only visibile inside that block. Therefore, since discountedPrice is declared in the for loop, it will not be visible anymore once the loop ends.
11. Disregarding the error in previous lines that const can't be reassigned, the finalPrice will be printed, because finalPrice is declared in the same block as the console.log statement (within the function block) and therefore can be accessed by the for loop and the console.log statement.
12. Assuming there's somehow no errors at all, I would expect an empty array to be returned, because the discounted is declared in the same block as the return statement (within the function block). However, since it is declared as a const, the value of discounted cannot be changed once it's assigned, therefore the empty array will be returned.
13. A. student.name
    B. student['Grad Year']
    C. stedunt.greeting()
    D. student['Favorite Teacher'].name
    E. student.courseLoad[0]
14. A. '32', because 2 is converted to a string and then is concatenated to '3'
    B. 1, because '3' is converted to a number and then 3 - 2 = 1
    C. 0, because 3 is a number, null is converted to a number which would be 0, then 3 + 0 = 0
    D. '3null', because '3' is a string, null is converted to a string which would be 'null', then is concatenated to '3'
    E. 3, because 3 is a number, true is converted to a number which would be 1, then 1 + 3 = 4
    F. 0, because false and null are both converted to number 0, then 0 + 0 = 0
    G. '3undefined, because '3' is a string, undefined is converted to a string which would be 'undefined', then is concatenated to '3'
    H. NaN, because undefined is converted to a number which would be NaN (not 0), then 33 - NaN = NaN
15. A. true, because string '2' is converted to number 2 and 2 > 1 is true
    B. false, because this is string comparison and first character of '2' < first character of '12' (which is '1') is false
    C. true, because '2' is converted to a number and 2 == 2 is true
    D. false, because === is a strict equality operator which compares without type conversion. Since 2 and '2' are two different types, they are not equal
    E. false, because true is converted to a number which would be 1, and 1 == 2 is false.
    F. true, because 2 is converted to a boolean which would be true because any non-zero values would be true, and true == true is true.
16. The main difference between "==" and "===" that "===" is a strict equality operator and does not type convert when comparing 2 values, whereas "==" is a regular equality operator and automatically type converts under certain situations when comparing. For example, '2' == 2 is true but '2' === 2 is false.
17. 'How are you', because in the first if statement true will be converted to number, which is 1. Since 2 == 1 is false, therefore the first if statement will not be executed. In the else if statement, any non-zero numberic value will evaluate to true, therefore the else if statement will be executed and the else statement will be skipped.
19. [6, 8, 10]. When modifyArray is called, it first creates a new empty array to store the modified input array and return it. The for loop will actually compute the value that will be pushed into the new array. For example, the first element of the original array, 1, will be passed into the callback function, in this case it will be the doSomething function that we defined and passed into the modifyArray function. doSomething then takes the input number (1) add 2 and feed it to another callback function, which is the inline function we defined that will return the input times 2. Therefore (1 + 2) * 2 = 3 * 2 = 6. Similarly, (2 + 2) * 2 = 8, and (3 + 2) * 2 = 10. The output is [6, 8, 10]
21. 1 4 3 2, because 1 and 4 are not delayed at all and they will be printed first in the order they are executed. 3 is printed out next because it has less delay than console.log(2)

