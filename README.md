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


module ex21(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule


module p1(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

**RTL realization**

<img width="2552" height="1352" alt="ex21(1)" src="https://github.com/user-attachments/assets/df570f77-9d13-453e-8cb6-3047ee850730" />


<img width="2558" height="1359" alt="p1" src="https://github.com/user-attachments/assets/17b3b77b-9068-4a70-8c2b-9f066738e11b" />


**RTL**

<img width="2531" height="1355" alt="e21(1)1" src="https://github.com/user-attachments/assets/a4d19390-99b0-434e-aa0e-68a27947a758" />

<img width="2560" height="1353" alt="p12" src="https://github.com/user-attachments/assets/86d4033c-6f4a-4817-9a4a-4dd52cc32455" />


**Timing Diagram**
<img width="2531" height="1355" alt="e21(1)1" src="https://github.com/user-attachments/assets/75a47b0e-517a-4820-aa1b-2055bc467445" />
<img width="2560" height="1353" alt="p12" src="https://github.com/user-attachments/assets/b3960681-2205-49b4-8b98-36eec4ca0d55" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

