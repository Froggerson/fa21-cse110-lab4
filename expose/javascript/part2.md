1. At line 12, 3 is printed. We iterate through the for-loop three times, and which means that i gets incremented 3 times. Since i was declared using var, its scope is within the function discountPrices and we can print it outside of the for loop.
2. At line 13, 150 will be printed. We are printing discountedPrice, which was declared using var, so we have access to it outside of the for loop. discoutedPrice is updated each time that the for loop is run, so the last value of discountedPrice that is printed will be from the last iteration of the loop. In this case, prices[i] (where i = 2) would be 300, and we multiply that by 0.5 to get 150.
3. 150 will be printed. finalPrice was declared outside of the for-loop but within the function discountPrices so we can still access it within the function. It rounds off the value of discountedPrice so the value of finalPrice should be similar to it. We get 150 because that is the last value of finalPrice before the for-loop ended. This is similar to question 2.
4. It returns a list of numbers, specifically [ 50, 100, 150 ], because we were appending the discounted values of the original list to a new list called discounted. The value of that new list is returned. Note that we can not access discounted outside of the function, but since we returned its value we can still use it in some shape or another.
5. We get an error because i was declared with let within the scope of the for loop. It does not exist outside of the for loop, so when we tried to access it there we received an error.
6. We get an error because discountedPrice was declared with let within the scope of the for loop. It does not exist outside of the for loop, so when we tried to access it there we received an error.
7.  150 is printed. Although finalPrice is declared with let, it was declared within the scope of the function discountPrices so we can access it anywhere within the same function. finalPrice calculates the value at prices[i] with the discount applied. The value that is printed is from the last iteration of the for loop which is the discount of the last value in prices (300), so we get 150 (300 * 0.5).
8. It returns a list of numbers, specifically [ 50, 100, 150 ], because we were appending the discounted values of the original list to a new list called discounted. The value of that new list is returned. Note that we can not access discounted outside of the function, but since we returned its value we can still use it in some shape or another.
9. We get an error because i was declared with let within the scope of the for loop. It does not exist outside of the for loop, so when we tried to access it there we received an error.
10. 3 is printed because we defined the variable length with const within the scope of the same function that we declared it in, thus we still have access to it. The length of prices is 3 because it holds 3 elements in it. We also didn't get any errors because we didn't change the value of prices.
11. It returns a list of numbers, specifically [ 50, 100, 150 ], because we were appending the discounted values of the original list to a new list called discounted. The value of that new list is returned. Even though discounted was declared using const, we were able to append values to the new list since the variable discounted holds the address of the new list in memory. Since we never changed the address that discounted is pointing to, we don't get any errors. Note that when we append things to discounted, we add things to the list it is pointing to in memory.
12. A. student.name
    B. student['Grad Year']
    C. student.greeting();
    D. student['Favorite Teacher'][name]
    E. student.courseLoad[0]
13. A. '32' - 2 evaluates to '2', so we concatenate the strings together.
    B. 1 - '3' evaluates to 3, so we subtract normally.
    C. 3 - null evaluates to 0, so we add normally.
    D. '3null' - null evaulates to 'null', so we concatenate the strings together.
    E. 4 - true evaluates to 1, so we add 1 and 3 together.
    F. 0 - Both false and null evaluate to 0 so we add 0 and 0.
    G. '3undefined' - undefined becomes the string 'undefined', so we add the strings together.
    H. NaN - undefined converts to NaN because it is not a valid number and we are using a math operation. '3' becomes 3, but since undefined is not a valid number, subtracting the two will result in NaN.
14. A. true - '2' is converted to the number 2 because of JavaScript schenanigans, and since 2 is greater than 1, the condition is true.
    B. false - Both values are strings, so the values are compared letter by letter. Although '2' is numerically greater than '12', '2' is greater than '1' if we compare them letter by letter, so the condition is false.
    C. true - The '==' operator converts values to the same type, so '2' becomes 2, and since 2 is equal to 2, the comparison is true.
    D. false - '===' does not convert the values to different types. '2' is a string while 2 is a number, so they are not equal and the comparison returns false.
    E. false - true is evaluated to its numerical value, 1, due to the '==' operator .1 is not equal to 2 so false is returned.
    F. true  - 2 is converted to its boolean value, true. true is equal to true, so true is returned.
15. '==' converts values to the same type if necessary and then does a comparision while '===' does not. In other words, '===' is more strict with the type of the values that it is comparing.
16. See part2-question16.js
17. The result is [2, 4, 6]. I'm sorry but I haven't taken a nap today so this may sound incoherent. Ok, so we call modifyArray with the parameters [1,2,3] and doSomething. doSomething is a function that does something. That something is muliplying the parameter, a number, by 2 and returning it. In modifyArray we create a nifty new array call newArr. Nice, right? Then we basically iterate through the array we put in the parameter ([1,2,3]). For each value we iterate through the array, we call doSomething on it and push it to the new array. doSomething multiplies the value by two, so we basically multiply each value in [1,2,3] by 2, push it to a new array, and then return that new array. Nice.  
18. See part2-question18.js
19. 1
    4
    3
    2