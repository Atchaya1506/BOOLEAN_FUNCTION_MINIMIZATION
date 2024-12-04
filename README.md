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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/
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




**RTL **
funt1:![ex 2 rtl](https://github.com/user-attachments/assets/b94334e8-fe45-4172-9785-6947e535a3f5)
funct2:![2 1](https://github.com/user-attachments/assets/caa54cbb-3153-440c-9017-306ce8e2710d)


**Output:**
funct1:![ex 2](https://github.com/user-attachments/assets/8bf237da-b38b-4c19-98d4-79e519164ead)

funct2:![2 1 DE](https://github.com/user-attachments/assets/313b4f4a-1ce9-495e-89d8-1894bbf8748d)



**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

