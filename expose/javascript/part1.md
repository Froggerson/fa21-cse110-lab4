1. values added: 20
2. final result: 20
3. values added: 20
4. Nothing is printed, because there is an error! Variables defined with let has a block scope. Since we defined the variable 'result' in the if-statement block, it can not be accessed outside of the if-statement. Since we tried to do that, we got an error.
5. Error. Variables declared with const can not be reassigned another value. Since we tried to set result equal to num1 + num2, we received an error.
6. Nothing is printed here because we received an error earlier when we tried to reassign the variable result.