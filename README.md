# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit
Implementation-of-Half-Adder-and-Full-Adder-circuit

# AIM:

To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

# Equipments Required:
Hardware – PCs, Cyclone II , USB flasher. Software – Quartus prime.

# Theory

Adders are digital circuits that carry out addition of numbers.

# Half Adder

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB
![Screenshot (72)](https://user-images.githubusercontent.com/119476322/215163578-4030d1cb-993c-4b37-b83a-d88929d7d6a1.png)

# Full Adder

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

![Screenshot (73)](https://user-images.githubusercontent.com/119476322/215163628-78424147-30b4-4ea7-80ef-4923b2305884.png)

# Procedure

1.Using xor,and,not,or gates and wires ,construct Half Adder.

2.Repeat same steps to construct for Full Adder.

3.Find RTL logic and timing diagram for both Adders

4.End the program

# Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Sivaramakrishnan B
RegisterNumber:22006798

Half Adder

module HalfAdder(a,b,sum,carry);

input a,b;

output sum,carry;

xor(sum,a,b);

and(carry,a,b);

endmodule

Full Adder

module FullAdder(a,b,c,sum,carry);

input a,b,c;

output sum,carry;

assign sum = ((a^b)^c);

assign carry = ((a&b)|(b&c)|(c&a));

endmodule
```

# Output:

# Half Adder

# Truthtable

![Screenshot (74)](https://user-images.githubusercontent.com/119476322/215163760-0178cade-e8ea-474b-acee-2724315845e7.png)

# RTL realization

![Screenshot (75)](https://user-images.githubusercontent.com/119476322/215163839-6e8237fc-e0ae-48f4-a9b8-25939344d9ad.png)

# Timing diagram

![Screenshot (76)](https://user-images.githubusercontent.com/119476322/215163875-bcdc9a57-67f5-4574-b7d5-9cf5aafc62e3.png)

# Full Adder

# Truthtable

![Screenshot (77)](https://user-images.githubusercontent.com/119476322/215163907-4be75b6b-ed12-40ca-bd22-fe93b5fe049c.png)

# RTL realization
![Screenshot (78)](https://user-images.githubusercontent.com/119476322/215163926-15d0af81-c100-40b1-8ee9-9ae1a48f964f.png)

# Timing Diagram 

![Screenshot (79)](https://user-images.githubusercontent.com/119476322/215163958-64c83cc4-2547-4ed1-9095-aeb9952205f5.png)

# Result:
Thus,design of half adder and full adder circuit and verify its truth table in Quartus using Verilog programming is executed successfully
