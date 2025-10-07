# BOOLEAN_FUNCTION_MINIMIZATION

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

module exe2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)| (~a&b&d)| (a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule 

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: SANJAI S J

RegisterNumber: 25007032


**RTL realization**

<img width="819" height="654" alt="Screenshot 2025-10-07 152527" src="https://github.com/user-attachments/assets/a0e5f9f0-5e7e-442e-939e-7bfb19d3eee4" />

**Output:**

**RTL**

<img width="954" height="594" alt="Screenshot 2025-10-07 152437" src="https://github.com/user-attachments/assets/170ac6aa-5720-4190-b78f-884671972cb9" />

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

