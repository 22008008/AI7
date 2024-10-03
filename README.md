# Ex.No: 7 Logic Programming – Logic Circuit Design
```
NAME : Sri Ranjani Priya P
REGISTER NUMBER : 212222220049
```

# AIM:
To write a logic program to design a circuit like half adder and half subtractor.

# Algorithm:
Start the Program
Design a AND gate logic if both inputs are 1 then output is 1.
Design a OR gate logic if any one of input is 1 then output is 1.
Design a XOR gate logic if both inputs are different then output is 1.
Design a NOT gate logic if input is 0 then output is 1.
Design a half adder and half subtractor using the rules.
Test the logic.
Stop the program.

# Program:
```% Define the XOR gate
xor(0, 0, 0).
xor(0, 1, 1).
xor(1, 0, 1).
xor(1, 1, 0).

% Define the AND gate
and(0, 0, 0).
and(0, 1, 0).
and(1, 0, 0).
and(1, 1, 1).

% Define the NOT gate
not(0, 1).
not(1, 0).

% Define the half-subtractor circuit
half_subtractor(A, B, Diff, Borrow) :-
    xor(A, B, Diff),
    not(B, NotB),
    and(A, NotB, Borrow).

% Define the half-adder circuit
half_adder(A, B, Sum, Carry) :-
    xor(A, B, Sum),
    and(A, B, Carry).
```
# Output:
OUTPUT FOR HALF ADDER:
![image](https://github.com/user-attachments/assets/ed14c129-3c4e-4d06-8aba-55392369e7a4)

OUTPUT FOR HALF SUBTRACTOR:
![image](https://github.com/user-attachments/assets/76ad126c-f443-4654-8a40-1382fa0ea824)


# Result:
Thus the truth table of circuit verified sucessfully.
