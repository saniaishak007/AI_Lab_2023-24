
# Ex.No: 10  Logic Programming –  Simple queries from facts and rules
### DATE:                                                                            
### REGISTER NUMBER : 
### AIM: 
To write a prolog program to find the answer of query. 
###  Algorithm:
 Step 1: Start the program <br> 
 Step 2: Convert the sentence into First order Logic  <br> 
 Step 3:  Convert the sentence into Horn clause form  <br> 
 Step 4: Add rules and predicates in a program   <br> 
 Step 5:  Pass the query to program. <br> 
 Step 6: Prolog interpreter shows the output and return answer. <br> 
 Step 8:  Stop the program.
### Program:
### Task 1:
Construct the FOL representation for the following sentences <br> 
1.	John likes all kinds of food.  <br> 
2.	Apples are food.  <br> 
3.	Chicken is a food.  <br> 
4.	Sue eats everything Bill eats. <br> 
5.	 Bill eats peanuts  <br> 
   Convert into clause form and Prove that John like Apple by using Prolog. <br> 
### Program:
```
likes(steve,X):-easycourse(X).
hard(science).
easycourse(X):-dept(havefun,X).
dept(havefun,bk301).
```

### Output:
<img width="949" height="311" alt="Screenshot 2025-09-06 140950" src="https://github.com/user-attachments/assets/a4219ddb-84c3-4883-a574-79c40fe17a23" />

### Task 2:
Consider the following facts and represent them in predicate form: <br>              
1.	Steve likes easy courses. <br> 
2.	Science courses are hard. <br> 
3. All the courses in Have fun department are easy <br> 
4. BK301 is Have fun department course.<br> 
Convert the facts in predicate form to clauses and then prove by resolution: “Steve likes BK301 course”<br> 

### Program:
```
likes(john,X):-food(X).
food(apple).
food(chicken).
eats(sue,X):-eats(bill,X).
eats(bill,peanuts).
```

### Output:
<img width="946" height="266" alt="Screenshot 2025-09-06 141024" src="https://github.com/user-attachments/assets/385c79dc-fc17-4d64-8581-403705a5dc7e" />

### Task 3:
Consider the statement <br> 
“This is a crime for an American to sell weapons to hostile nations. The Nano , enemy of America has some missiles and its missiles were sold it by Colonal West who is an American” <br> 
Convert to Clause form and prove west is criminal by using Prolog.<br> 
### Program:
```
crime(X):-american(X),weapon(Y),hostile(Z,X),sells(X,Y,Z).
weapon(Y):-missile(Y).
hostile(B,A):-enemy(A,B).
enemy(A,B):-hostile(B,A).
enemy(nano,west).
sells(west,Y,nano):-owns(nano,Y),missile(Y).
owns(nano,m1).
missile(m1).
american(west).
```
### Output:
![Screenshot 2025-09-06 143331 1](https://github.com/user-attachments/assets/d81b65d3-06d3-4f5a-8285-e389859c9bbf)

### Result:
Thus the prolog programs were executed successfully and the answer of query was found.
```
