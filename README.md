# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
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

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: DIVYAVARSHINI K.S
RegisterNumber: 212222050012 
Half Adder
module ex02_1(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
endmodule
Full Adder
module ex02(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum =((a^b)^c);
assign carry =((a&b)|(b&c)|(c&a));
endmodule
*/
![WhatsApp Image 2023-03-30 at 7 24 39 PM](https://user-images.githubusercontent.com/128978058/228860895-da920dd3-af44-48b6-aca2-0da1dc428837.jpeg)

RTL 
![WhatsApp Image 2023-03-30 at 7 24 39 PM (1)](https://user-images.githubusercontent.com/128978058/228861044-5f6d73a1-d956-4f45-a227-a5ad2e5b46d5.jpeg)


TIMMING DIAGRAM 

![WhatsApp Image 2023-03-30 at 7 24 39 PM (2)](https://user-images.githubusercontent.com/128978058/228861210-0382bc27-308a-4b00-a9d3-976b5f8afaec.jpeg)

TRUTH TABLE 

![WhatsApp Image 2023-03-30 at 7 24 40 PM](https://user-images.githubusercontent.com/128978058/228861334-260b5bb0-e0ab-42b9-8ea4-fce0162984df.jpeg)

RESULT:
Thus the half adder and full adder circuit was succesfully implemented














