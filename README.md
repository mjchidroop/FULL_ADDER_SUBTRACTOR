# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)
<img width="429" height="395" alt="image" src="https://github.com/user-attachments/assets/9187c1aa-030a-4628-97ed-17a0ba9abf89" />
<img width="300" height="144" alt="image" src="https://github.com/user-attachments/assets/376ccaa7-e9a6-4153-a5d1-a2538a33c7a6" />

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)
<img width="438" height="393" alt="image" src="https://github.com/user-attachments/assets/8db5f3f4-ec33-4810-9e4c-c7a26810c701" />
<img width="916" height="397" alt="image" src="https://github.com/user-attachments/assets/0bec1e3c-60ae-48bb-87e8-d2b60278a38b" />

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable** 
<img width="440" height="815" alt="image" src="https://github.com/user-attachments/assets/29f3683b-a3ea-42ea-94f5-41852d6cc4ac" />


**Procedure** 
1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.


**Program:**

```
NAME: Chidroop M J regno: 212225240029
```
```verilog
module Exp4(A,B,C,S1,C1,D1,B1);
input A,B,C;
output S1,C1,D1,B1;
assign S1=A^B^C;
assign C1=A&B|A&C|B&C;
assign D1=A^B^C;
assign B1=~A&(C|B)|B&C;
endmodule
```



**RTL Schematic** 
<img width="946" height="515" alt="image" src="https://github.com/user-attachments/assets/27f9449b-f4bf-4a7c-a7a3-d4190e0b5954" />

**Output Timing Waveform** 
<img width="948" height="505" alt="image" src="https://github.com/user-attachments/assets/5c7cdbb5-f3f1-4838-8d53-e5ff8d3a3d3e" />

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



