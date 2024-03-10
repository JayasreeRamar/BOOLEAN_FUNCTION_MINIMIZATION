# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Theory**
A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module combinationalcircuit(A,B,C,D,F1);
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

#### Developed by: Jayasree R
#### RegisterNumber: 212223230087


**RTL realization**

![285831617-8766d4a1-0593-4b06-a5f4-8c977e44b4ad](https://github.com/JayasreeRamar/BOOLEAN_FUNCTION_MINIMIZATION/assets/138972962/48d79fa0-ed09-4411-853d-5573d9de908e)

**Output:**

**Timetable**

![285832032-236326de-e839-4fad-908b-bb236e0a13dd](https://github.com/JayasreeRamar/BOOLEAN_FUNCTION_MINIMIZATION/assets/138972962/67d63c8b-e81d-4fa2-b2ec-44bfdb3bb7de)

**Timing Diagram**

![285832328-c7532fe5-12ef-476d-a070-ab42a2ea7636](https://github.com/JayasreeRamar/BOOLEAN_FUNCTION_MINIMIZATION/assets/138972962/1577ec82-56d9-4f62-929b-3d7cc48edfd0)

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


