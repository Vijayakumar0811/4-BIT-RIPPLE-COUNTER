# 4-BIT-RIPPLE-COUNTER

**EXP12: 4 BIT RIPPLE COUNTER**

NAME: VIJAYAKUMAR S

REG NO: 24900562

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**

 1. Type the program in Quartus software.

2. Compile and run the program.

3. Generate the RTL schematic and save the logic diagram.

4. Create nodes for inputs and outputs to generate the timing diagram.

5. For different input combinations generate the timing diagram.


**PROGRAM**

 Program for 4 Bit Ripple Counter and verify its truth table in quartus using Verilog programming.

 module bitrip (

   input wire clk,  
   
   output reg [3:0] count 

);

always @(posedge clk) begin

   if (count == 4'b1111)
      
       count <= 4'b0000;
   
   else
      
       count <= count + 1;

end

endmodule 


 Developed by: VIJAYAKUMAR.S
 
 RegisterNumber:24900562


**RTL LOGIC FOR 4 Bit Ripple Counter**
![4bitrip](https://github.com/user-attachments/assets/3ca7e6fd-69b2-4a38-b0ef-9bc06c8f948a)

**TIMING DIGRAMS FOR 4 Bit Ripple Counter**
![4bitripple](https://github.com/user-attachments/assets/15c72512-bbd7-416f-87b5-9f0479e6441c)

**RESULTS**

Thus the  4 Bit Ripple Counter using verilog is implemented and their functionality using their functional tables
 is verified.
