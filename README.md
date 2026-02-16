<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/49a233a7-73e4-4793-ad9c-7159b980b361" /><img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/49a233a7-73e4-4793-ad9c-7159b980b361" /># BOOLEAN_FUNCTION_MINIMIZATION

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
```
module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = (~a & ~b & ~c & ~d) |
            (a & ~c & ~d) |
            (~b & c & ~d) |
            (~a & b & c & d) |
            (b & ~c & d);
assign f2 = (x & ~y & z) |
            (~x & ~y & z) |
            (~w & x & y) |
            (w & ~x & y) |
            (w & x & y);
endmodule

```

Developed by:Rajalakshmi V RegisterNumber:25016476




**Output:**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/dc41826b-950f-4997-8ebc-ff17e5e3b887" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/dc41826b-950f-4997-8ebc-ff17e5e3b887" />

**RTL**
<img width="1915" height="1079" alt="image" src="https://github.com/user-attachments/assets/81fb7b07-5c8a-499e-b89f-c0980377e6cf" />
<img width="1915" height="1079" alt="image" src="https://github.com/user-attachments/assets/81fb7b07-5c8a-499e-b89f-c0980377e6cf" />
Truth Table:

<img width="483" height="292" alt="Screenshot 2025-12-10 110440" src="https://github.com/user-attachments/assets/9116aafe-0299-4bbc-808e-2b39555d4353" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

