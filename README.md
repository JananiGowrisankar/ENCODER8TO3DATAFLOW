### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**

/* write all the steps invloved */

**PROGRAM**
```
/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by:Janani G 
RegisterNumber:24009971
*/
module exp5 (din, a,b, c);
input [0:7] din;
output a,b,c;
assign a=(din[4]| din[5]| din[6 ]| din[7]); 
assign b=(din[2]| din[3]| din[6]| din[7]); 
assign c=(din[1]| din[3]| din[5 ]| din[7]);
endmodule
```
**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

![exp51](https://github.com/user-attachments/assets/a4a016f8-9d52-448c-90d2-9f31ef585191)


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

![exp52](https://github.com/user-attachments/assets/697b524d-ca99-4b74-a152-71123147b110)


**RESULTS**

Then the basic logic gates are satisfied and the truth table is verified.


