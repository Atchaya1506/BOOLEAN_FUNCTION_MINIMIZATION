# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
Developed by:ATCHAYA B

RegisterNumber:24900268

fuct1:

module ex(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule


funt2:

module booleanfunction(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule




**RTL ** realization
funt1:![ex 2 rtl](https://github.com/user-attachments/assets/b94334e8-fe45-4172-9785-6947e535a3f5)
funct2:![2 1](https://github.com/user-attachments/assets/caa54cbb-3153-440c-9017-306ce8e2710d)


**Output**


![Screenshot 2024-12-05 111914](https://github.com/user-attachments/assets/663cc4a6-92a6-43d7-bd91-682d02da33d2)

![Screenshot 2024-12-05 111934](https://github.com/user-attachments/assets/0dfb9c1d-be25-41bc-83e3-2b704d83b54d)



**Timing Diagram**

funct 1:
![ex 2](https://github.com/user-attachments/assets/9cbce2c8-30a7-44f6-ae1d-f887fb18e929)

funct 2:

![2 1 DE](https://github.com/user-attachments/assets/3e392e0a-13ac-4bf6-819e-96d83a8e4b83)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

