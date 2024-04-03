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

**Half adder:**

![image](https://github.com/VimalasahanaW/HALF_ADDER_SUBTRACTOR/assets/144870812/be210279-df41-43bf-b46d-09a9399d813b)





**Half subtractor:**




![image](https://github.com/VimalasahanaW/HALF_ADDER_SUBTRACTOR/assets/144870812/b25653aa-0f82-4768-b0f8-84e8736846b2)




**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.*/

Developed by:vimala sahana W RegisterNumber:212223040241

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
**RTL Schematic half adder:**
![image](https://github.com/VimalasahanaW/HALF_ADDER_SUBTRACTOR/assets/144870812/465b488c-0cc1-41d8-a9b5-a68d06093e92)

**half subtractor:**


![image](https://github.com/VimalasahanaW/HALF_ADDER_SUBTRACTOR/assets/144870812/deabf2ea-620c-41ee-86ff-efbc9cad5fcf)



**Output/TIMING Waveform**


**half adder:**


![image](https://github.com/VimalasahanaW/HALF_ADDER_SUBTRACTOR/assets/144870812/d8745a31-c1a9-46ae-a135-62d2dc8470f8)


**half subtractor:**


![image](https://github.com/VimalasahanaW/HALF_ADDER_SUBTRACTOR/assets/144870812/6cebbaf7-595d-4afb-9478-b49ea3359420)


**Result:**
Thus the half subtractor and half adder circuits are designed and the truth tables is verified using quartus software.
