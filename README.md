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
1)
module logic_function(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a&b&d)|(a&b&~c));
endmodule
```
```
2)
module EXP2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Monika.A 
RegisterNumber:212224240094

**TRUTH TABLE**
![EXP2(1)](https://github.com/user-attachments/assets/77ac30e0-5853-4db8-adbe-2d7a965ff949)
![EXP2(2)](https://github.com/user-attachments/assets/e6f7a980-379c-4fe0-b2ef-1352c3cbdef1)

**RTL realization**
![EXP2(1)](https://github.com/user-attachments/assets/8560031f-30af-4bee-a285-b7ec0995ed5d)
![EXP2(2)](https://github.com/user-attachments/assets/e81b1f1b-c871-474a-bc06-d83d70fb09b9)

**RTL**
![EXP2(1)](https://github.com/user-attachments/assets/e9a06691-59ea-418d-897d-ad90dd93b0bd)
![EXP2(2)](https://github.com/user-attachments/assets/be0dc2ff-6954-43fa-b837-fc8e2b57f740)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

