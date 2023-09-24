# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus. F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime

## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

## Procedure
Step 1: Create a project with required entities.

Step 2: Create a module along with respective file name.

Step 3: Run the respective programs for the given boolean equations.

Step 4: Run the module and get the respective RTL outputs.

Step 5: Create university program(VWF) for getting timing diagram.

Step 6: Give the respective inputs for timing diagram and obtain the results.
## Program:
```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: MOHAMED AZEEM N
RegisterNumber:  212222110026

module Exp02(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule

```
## Output

## RTL
![Screenshot (122)](https://github.com/mohamedazeem33/Experiment--02-Implementation-of-combinational-logic-/assets/121040764/d30dd03a-c9ed-4138-9fc6-7267f30d807c)

## Truth Table
![Screenshot (123)](https://github.com/mohamedazeem33/Experiment--02-Implementation-of-combinational-logic-/assets/121040764/f770bf3f-baae-4f28-b5da-5efb81e4ca98)

## Timing Diagram
![Screenshot (124)](https://github.com/mohamedazeem33/Experiment--02-Implementation-of-combinational-logic-/assets/121040764/e9259af6-1973-4423-9057-480125097bb7)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
