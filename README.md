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
module boolean(A,B,C,D,F1);
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

Developed by: RegisterNumber:212223110062



**Output:**
![image](https://github.com/Vigneshv-23/BOOLEAN_FUNCTION_MINIMIZATION/assets/110780412/3ca20bdb-f677-4c46-be64-ede6b3b993c0)


**RTL**
![image](https://github.com/Vigneshv-23/BOOLEAN_FUNCTION_MINIMIZATION/assets/110780412/cb50880a-2b81-4121-96be-1cddc497876d)


**Timing Diagram**
![image](https://github.com/Vigneshv-23/BOOLEAN_FUNCTION_MINIMIZATION/assets/110780412/105d011f-b5c8-4f21-8592-1c397527d645)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

