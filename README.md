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
Developed by:SABARI S 
RegisterNumber:  212222240085
*/
## HALF ADDER:
```
module exp33(a,b,s,c);
input a,b;
output s,c;
assign s=a^b;
assign c=a&b;
endmodule
```
## FULL ADDER:
```
module ass3(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=a^b^c;
assign carry= ((a&b)|(b&c)|(c&a));
endmodule
```

Logic symbol & Truthtable
RTL realization
### Output:
### RTL
## HALF ADDER

![264913765-084d609b-1bb0-4f47-82fe-3fb1dda94395](https://github.com/SABARI005/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118660461/57b51d3f-d848-4faa-8d26-d2ea4fe0365e)
## FULL ADDER
![264913797-6ca1e10c-a439-49f7-b7cb-cb7ed7b5e66e](https://github.com/SABARI005/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118660461/24b3d98a-856d-4b3c-b0f6-94b8c50c4393)
### TIMING DIAGRAM
## HALF ADDER
![264914200-95eccf36-94f9-4925-ad15-82c9579880aa](https://github.com/SABARI005/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118660461/b70caff0-5158-451d-a511-6ed4d605b773)

## FUL ADDER

![264913964-863312c7-17df-4b4c-9958-768cbbcf34e6](https://github.com/SABARI005/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118660461/7ace7d75-78c1-48a5-9ec0-4226d6c4e847)

### TRUTH TABLE 
## HALF ADDER

![264914641-9cd28690-b0b2-4e1f-8f6a-dcf9a657d344](https://github.com/SABARI005/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118660461/ec3a078b-e401-497f-8048-beabd2cdbf6c)

## FULL ADDER

![264914661-bb1b445a-65fa-4c1f-80fe-aca2993690f6](https://github.com/SABARI005/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118660461/9675f1e5-6056-4d20-b70f-6a8b7352563d)


### Result:
Thus the half adder and full adder are studied and the truth table for different logic gates are verified.
