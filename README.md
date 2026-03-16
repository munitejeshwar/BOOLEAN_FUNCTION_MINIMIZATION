# BOOLEAN_FUNCTION_MINIMIZATION
DEVELOPED BY:K Muni tejeshwar
REGISTER NUMBER:212223040102

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:MANIKANDAN M
RegisterNumber: 212224040183
```
module exp_2(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule
```
**truth table:**

<img width="557" height="851" alt="image" src="https://github.com/user-attachments/assets/aa6c7b6e-57ac-459a-8e52-43825bc484c4" />
<img width="560" height="852" alt="image" src="https://github.com/user-attachments/assets/507bde60-7bb1-40a5-951f-24f1e5808e7f" />

**Output:**
**RTL realization**
<img width="1920" height="1080" alt="Screenshot (578)" src="https://github.com/user-attachments/assets/46634cef-6fe2-40fd-84ef-075bbcded00b" />

**Timing Diagram**
<img width="1920" height="1080" alt="Screenshot (579)" src="https://github.com/user-attachments/assets/98fad2d0-b72c-4c72-bde2-1dfb949b927e" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
