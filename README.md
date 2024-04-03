# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**
## Half adder:
![image](https://github.com/StarbiyaS/HALF_ADDER_SUBTRACTOR/assets/144870533/95d0c566-ccba-48af-b3ae-212014fb5b0c)

## Half subtractor:
![image](https://github.com/StarbiyaS/HALF_ADDER_SUBTRACTOR/assets/144870533/27c93456-4314-417d-a25d-b8c79ca80453)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:STARBIYA S RegisterNumber:212223040208

**half adder**
```
module exp3(sum, carry,a,b); 
input a,b; 
output sum,carry; 
xor sum1(sum,a,b); 
and carry1(carry,a,b); 
endmodule
```

**half subtractor**
```
 module exp3(diff,carry,a,b);
 input a,b;
 output diff,carry;
 xor(diff,a,b);
 assign carry=(~a)&b;
 endmodule
```
**RTL Schematic**
**half adder**

![image](https://github.com/StarbiyaS/HALF_ADDER_SUBTRACTOR/assets/144870533/95e18de2-fa1f-4b2d-93ba-47bbea65f6de)

**half subtractor**

![image](https://github.com/StarbiyaS/HALF_ADDER_SUBTRACTOR/assets/144870533/a7023900-acee-429e-9633-045d2c973a79)


**Output/TIMING Waveform**

## half adder
![image](https://github.com/StarbiyaS/HALF_ADDER_SUBTRACTOR/assets/144870533/59a57533-5dd4-43a9-9eb8-82c26bfec17c)


## half subtractor
![image](https://github.com/StarbiyaS/HALF_ADDER_SUBTRACTOR/assets/144870533/f457704c-358b-4c38-a3cd-5a5726c425cd)

**Result:**
 Thus the half subtractor and half adder circuits are designed and the truth tables is verified using quartus software.
