
# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
# AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

# Equipments Required:
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
/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

## HALF ADDER:

module ex03(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum=a^b;

assign carry=a&b;

endmodule
## FULL ADDER:

module fulladder(a,b,cin,sum,carry); 

input a,b,cin;

output sum,carry;

assign sum=a^b^cin;

assign carry=(a&b)|((a^b)&cin);

endmodule */

# Output:
## RTL
### HALF ADDER
![image](https://github.com/nivetharajaa/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120543388/40b2ca00-122d-4323-b051-b0472cc24475)
### FULL ADDER 
![image](https://github.com/nivetharajaa/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120543388/bcabc7cc-d54f-47a2-b0b2-5549a3f0bbc1)

# 2.TRUTH TABLE
### HALF ADDER
![image](https://github.com/nivetharajaa/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120543388/086036e1-ddca-4365-8ee1-c2947e3696d7)
### FULL ADDER
![image](https://github.com/nivetharajaa/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120543388/66e53013-6901-4da9-af28-6cd49335168e)
# 3.WAVEFORM
### HALF ADDER 
![image](https://github.com/nivetharajaa/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120543388/8888edff-9907-4bd9-a5f3-e6651a18719f)
### FULL ADDER 
![image](https://github.com/nivetharajaa/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120543388/3549ec33-9429-4237-b79c-e040c8c63d1d)

# Result:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.

