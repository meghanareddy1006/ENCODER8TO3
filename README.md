# ENCODER8TO3
# Aim:
To simulate and synthesis encoder using Xilinx ISE.

# Apparatus Required:
Xilinx 14.7 Spartan6 FPGA

# Procedure:
STEP:1 Start the Xilinx navigator, Select and Name the New project. STEP:2 Select the device family, device, package and speed. STEP:3 Select new source in the New Project and select Verilog Module as the Source type. STEP:4 Type the File Name and Click Next and then finish button. Type the code and save it. STEP:5 Select the Behavioral Simulation in the Source Window and click the check syntax. STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table. STEP:7 Select the Implementation in the Sources Window and select the required file in the Processes Window. STEP:8 Select Check Syntax from the Synthesize XST Process. Double Click in the FloorplanArea/IO/Logic-Post Synthesis process in the User Constraints process group. UCF(User constraint File) is obtained. STEP:9 In the Design Object List Window, enter the pin location for each pin in the Loc column Select save from the File menu. STEP:10 Double click on the Implement Design and double click on the Generate Programming File to create a bitstream of the design.(.v) file is converted into .bit file here. STEP:11 On the board, by giving required input, the LEDs starts to glow light, indicating the output.
![image](https://github.com/RESMIRNAIR/ENCODER3TO8/assets/154305926/824226c8-c767-44b5-ab35-26fed65b195e)
# Truth Table
![image](https://github.com/RESMIRNAIR/ENCODER3TO8/assets/154305926/e228c14b-b814-40c8-92eb-748d48570c04)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/ENCODER3TO8/assets/154305926/6fa5fe84-fe6f-472d-b9c0-e6dfa17413d3)
![image](https://github.com/RESMIRNAIR/ENCODER3TO8/assets/154305926/7d147e2a-ba03-4714-baee-17615c9c50c1)
# Program:
```
module encoder(d,a0,a1,a2);
input[7:0]d;
output a0,a1,a2;
assign a2=d[7]|d[6]|d[5]|d[4];
assign a1=d[7]|d[6]|d[3]|d[2];
assign a0=d[7]|d[5]|d[3]|d[1];
endmodule
```
# output
![image](https://github.com/RESMIRNAIR/ENCODER8TO3/assets/163811142/806e2e98-f140-4d29-bdaa-46bfa5a0630b)
# Result
Hence encorder is verified

