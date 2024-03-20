# Ex. No: 6 PL/SQL program to perform addition and subtraction of two number 
### DATE: 
### AIM: To create PL/SQL program to perform addition and subtraction of two number.

### Steps:
1. Declare the variable a, b and necessary variables in Declare section.
2. Perform addition of two numbers
3. Perform subtraction of two numbers 
4. Display the result 
5. End the begin section.

### Program:
```
-- Create a PL/SQL block
DECLARE
    -- Declare variables to hold the numbers and results
    num1 NUMBER := 10;
    num2 NUMBER := 5;
    result_addition NUMBER;
    result_subtraction NUMBER;
BEGIN
    -- Perform addition
    result_addition := num1 + num2;
    
    -- Perform subtraction
    result_subtraction := num1 - num2;
    
    -- Display the results
    DBMS_OUTPUT.PUT_LINE('Addition: ' || result_addition);
    DBMS_OUTPUT.PUT_LINE('Subtraction: ' || result_subtraction);
END;
/
```

### Output:
![image](https://github.com/sandhyabalamurali/DBMS/assets/115525118/a1c39863-20a2-4165-aef4-69885f06000b)


### Result:
Thust the program was performed sucessfully.
