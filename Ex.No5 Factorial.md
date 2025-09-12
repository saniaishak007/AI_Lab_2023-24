# Ex.No: 5   Logic Programming – Factorial of number   
### DATE: 12-09-2025                                                                           
### REGISTER NUMBER : 212223060243
### AIM: 
To  write  a logic program for finding the factorial of given number using SWI-PROLOG. 
### Algorithm:
1. STEP 1: Start the program
2. STEP 2:  Write a rules for finding factorial of given program in SWI-PROLOG.
3.   a)	factorial of 0 is 1 => written as factorial(0,1).
4.   b)	factorial of number greater than 0 obtained by recursively calling the factorial    function.
5. STEP 3: Run the program  to find answer of  query.
6. STEP 4: Stop the program.

### Program:
```
fact(0,1).
fact(C,Res):-
    C > 0,
    A is C-1,
    fact(A,B),
    Res is C*B.
```
### Output:

<img width="954" height="416" alt="image" src="https://github.com/user-attachments/assets/f65ce173-9ec1-4f2a-97b6-5e9e018d9dfe" />


### Result:
Thus the factorial of given number was found by logic programming. 
