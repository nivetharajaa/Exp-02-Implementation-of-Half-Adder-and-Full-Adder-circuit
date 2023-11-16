
# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
## AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

# Procedure:
Connect the supply (+5V) to the circuit

Switch ON the main switch

If the output is 1, then the led glows.
 
# Program:
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

## HALF ADDER:
 ```
module ex03(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum=a^b;

assign carry=a&b;

endmodule
```
## FULL ADDER:
```
module fulladder(a,b,cin,sum,carry); 

input a,b,cin;

output sum,carry;

assign sum=a^b^cin;

assign carry=(a&b)|((a^b)&cin);

endmodule 
```
# Output:
## RTL
### HALF ADDER
![267680708-7567b145-1cc6-4b5f-b2cc-03649206c05f](https://github.com/nivetharajaa/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120543388/69532f0c-b4ec-42e1-b3e3-915eb60af526)

### FULL ADDER 
![279304704-512b65cd-e9a6-4ffe-8b25-a8ae1fceab3a](https://github.com/nivetharajaa/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120543388/3dd88bec-5f6e-452d-b286-a1a7167905dd)


# 2.TRUTH TABLE
### HALF ADDER
![267681222-e04a5ebd-468c-488f-9c95-9c26d49b42a7](https://github.com/nivetharajaa/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120543388/9849c5bf-690c-4b4b-b2c6-767fa4ab74ce)

### FULL ADDER
![267681375-c520bceb-ea5c-402d-9afb-40ec723f0aaf](https://github.com/nivetharajaa/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120543388/44ae5129-7db2-4441-bdf0-c176cc3e848b)

# 3.WAVEFORM
### HALF ADDER 
![267681757-0a222bc3-eef4-4876-b6ac-03b723e69442](https://github.com/nivetharajaa/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120543388/a0de74a9-3f13-450e-bcd4-a4b845f1108c)

### FULL ADDER 

![267682112-a4ce5d4c-d477-428a-a626-b46d1c60208d](https://github.com/nivetharajaa/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120543388/60fccd85-f5b8-430f-bfc9-4deae415effe)

# Result:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.

