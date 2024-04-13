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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:212222110015

```

module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
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


**RTL realization**

![319427331-4d407a87-3dc2-49e6-bea8-bb7683f1857d](https://github.com/Kamali22004796/BOOLEAN_FUNCTION_MINIMIZATION/assets/120567837/234a4d32-e8e0-482f-abfb-794c634a8c37)


**RTL**

![319427514-042b4487-4220-4e63-a855-f1475debf723](https://github.com/Kamali22004796/BOOLEAN_FUNCTION_MINIMIZATION/assets/120567837/f225ede6-3a42-4b3e-8d14-7d8b83c6b334)


**Logic Symbol and Truth table**
![319427043-ab520f8d-0d6f-4bb9-96e6-33968a037418](https://github.com/Kamali22004796/BOOLEAN_FUNCTION_MINIMIZATION/assets/120567837/9d7cb692-3168-4d3e-96ed-d42ded9b3de2)


![319427157-21cb2aef-7529-4ced-a473-68b7a9e53d62](https://github.com/Kamali22004796/BOOLEAN_FUNCTION_MINIMIZATION/assets/120567837/b1e95cec-1fd1-4837-9e28-644504977e1b)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

