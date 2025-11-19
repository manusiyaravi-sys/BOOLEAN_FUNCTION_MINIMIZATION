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


module ex22(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

**RTL realization**
<img width="2541" height="1342" alt="ex21 1" src="https://github.com/user-attachments/assets/96a5aa3f-161d-4c52-aad8-a7f93e229fc9" />
<img width="2552" height="1409" alt="ex22 1" src="https://github.com/user-attachments/assets/5cb05239-6c52-46c7-9f66-b03d51ce83bd" />



**RTL**
<img width="2539" height="1276" alt="ex21 2" src="https://github.com/user-attachments/assets/8838b2ab-9ce0-4480-9895-73e13b016a68" />
<img width="2550" height="1299" alt="ex22 2" src="https://github.com/user-attachments/assets/f2b8ac11-ae90-4427-b9e9-98b67c4dd59f" />


**Timing Diagram**
<img width="2539" height="1276" alt="ex21 2" src="https://github.com/user-attachments/assets/deb6c370-1363-4f75-ae25-5c3e1042b9f6" />
<img width="2550" height="1299" alt="ex22 2" src="https://github.com/user-attachments/assets/cd7cc7ac-ea95-425c-8884-1309e7d31ad2" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

