# Ex.No: 7  Logic Programming –  Logic Circuit Design
### DATE: 24/03/2024                                                                           
### REGISTER NUMBER : 212221040016
### AIM: 
To write a logic program to design a circuit like half adder and half subtractor.
###  Algorithm:
1. Start the Program
2. Design a AND gate logic if both inputs are 1 then output is 1.
3. Design a OR gate logic if any one of input is 1 then output is 1.
4. Design a XOR gate logic if both inputs are different then output is 1.
5. Design a NOT gate logic if input is 0 then output is 1.
6. Design a half adder and half subtractor using the rules.
7. Test the logic.
8. Stop the program.
### Program:
### HALF-ADDER:
```xor(0,1,1).
xor(0,0,0).
xor(1,0,1).
xor(1,1,0).
and(1,1,1).
and(0,0,0).
and(0,1,0).
and(1,0,0).
halfadder(A,B,Sum,Carry):-
xor(A,B,Sum),
and(A,B,Carry).
```
### HALF-SUBTRACTOR:
```xor(0,1,1).
xor(0,0,0).
xor(1,0,1).
xor(1,1,0).
and(1,1,1).
and(0,0,0).
and(0,1,0).
and(1,0,0).
not(0,1).
not(1,0).
or(0,1,1).
or(1,0,1).
or(0,0,0).
or(1,1,1).
halfsubtractor(A,B,Diff,Borrow):-
xor(A,B,Diff),
not(A,C),
and(C,B,Borrow).
```


### Output:
![image](https://github.com/DrUmaRaniV/AI_Lab_2023-24/assets/127651217/eacee6f1-be06-48b3-b01b-f84a318e67d4)
![image](https://github.com/DrUmaRaniV/AI_Lab_2023-24/assets/127651217/9c80e3f0-ad80-4225-8958-3281ec043c99)



### Result:
Thus the truth table of circuit verified sucessfully.
