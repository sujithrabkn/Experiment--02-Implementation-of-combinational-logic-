# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
 
## Equipments Required:
## Hardware 

PCs, Cyclone II , USB flasher

## Software

Quartus prime


## Theory
 
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output. F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

1.AND gate The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB Y= A.B

2.OR gate The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation. Y= A+B

## Procedure

1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.
## Program:

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

Developed by: SUJITHRA B K N

RegisterNumber: 212222230153 

```
module ex02(a,b,c,d,f1);
input a,b,c,d;
output f1;
wire x1,x2,x3,x4,x5;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a)&(~c)&(~d);
assign x3=(~b)&(c)&(~d);
assign x4=(~a)&(b)&(c)&(d);
assign x5=(b)&(~c)&(d);
assign f1=x1|x2|x3|x4|x5;
endmodule
```

## Output:

## RTL realization

![Screenshot 2023-08-26 083722](https://github.com/sujithrabkn/Experiment--02-Implementation-of-combinational-logic-/assets/119477857/5275beee-1f0f-4e4e-836c-937b3b4e025b)


## Truth table

![Screenshot 2023-08-26 094350](https://github.com/sujithrabkn/Experiment--02-Implementation-of-combinational-logic-/assets/119477857/b944d528-5089-4d10-8e8c-f7a1191b5742)

## Waveform

![ex02_De](https://github.com/sujithrabkn/Experiment--02-Implementation-of-combinational-logic-/assets/119477857/92fe8d1e-9f11-4913-b79f-b316888362da)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
