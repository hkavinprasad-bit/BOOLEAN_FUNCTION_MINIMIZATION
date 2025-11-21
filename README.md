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
```
module logic_function (a, b, c, d, w, x, y, z, f1, f2);

input a, b, c, d;
input w, x, y, z;
output f1, f2;

assign f1 = (~b & ~d) | (a & b & ~c) | (a & b & d);
assign f2 = (~y & z) | (x & y) | (w & z);

endmodule 
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:25017492


**RTL realization**

**Output:**
<img width="1919" height="1079" alt="Screenshot 2025-11-21 120134" src="https://github.com/user-attachments/assets/8135be63-e5f6-4102-b68f-7f5cbf749511" />

**RTL**
<img width="1919" height="1079" alt="Screenshot 2025-11-21 115932" src="https://github.com/user-attachments/assets/23e47377-9443-4ed7-bd94-eccbe35d2e23" />

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

