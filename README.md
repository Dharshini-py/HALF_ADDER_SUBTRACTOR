# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

<img width="476" height="448" alt="388822100-8372e670-4886-48bb-8369-820568a64d54" src="https://github.com/user-attachments/assets/66e85358-67bd-4c2f-8daa-3407b280a612" />


Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

HALF ADDER
<img width="426" height="282" alt="half adder" src="https://github.com/user-attachments/assets/5b99f3ea-a371-4145-b9b9-ec3b2d59e1a5" />

HALF SUBTRACTOR
<img width="415" height="316" alt="half subractor" src="https://github.com/user-attachments/assets/126baf12-f1b0-4ba2-bf51-98444d191f07" />


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

HALF ADDER           

module half_adder(sum, carry, a, b);     
  output sum;      
  output carry;        
  input a;     
  input b;      
  assign sum = a ^ b;         
  assign carry = a & b;       
endmodule     
 
HALF SUBTRACTOR          

module half_subtractor(diff, borrow, a, b);             
  output diff;       
  output borrow;     
  input a;          
  input b;         
  assign diff = a ^ b;      
  assign borrow = ~a & b;     
endmodule      


Developed by:DHARSHINI V          

RegisterNumber:25010872         

**RTL Schematic**

HALF ADDER

<img width="1920" height="1080" alt="Screenshot (24)" src="https://github.com/user-attachments/assets/ba756b01-38df-46cf-a529-16f5c18ac407" />

HALF SUBTRACTOR

<img width="1920" height="1080" alt="Screenshot (26)" src="https://github.com/user-attachments/assets/766651e9-af3d-44d9-8cdb-def517d8b8f3" />

**Output/TIMING Waveform**

HALF ADDER

<img width="1920" height="1080" alt="Screenshot (25)" src="https://github.com/user-attachments/assets/16190e92-2329-4c50-b29b-6cc2ea441500" />

HALF SUBTRACTOR

<img width="1920" height="1080" alt="Screenshot (27)" src="https://github.com/user-attachments/assets/cadd4dd9-e90f-4254-95f9-886ff9f97ca1" />

**Result:**

Program to design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming has been verified successfully.
