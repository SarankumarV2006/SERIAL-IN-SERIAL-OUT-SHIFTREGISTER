# SERIAL-IN-SERIAL-OUT-SHIFTREGISTER

**AIM:**

To implement  SISO Shift Register using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**SISO shift Register**

A Serial-In Serial-Out shift register is a sequential logic circuit that allows data to be shifted in and out one bit at a time in a serial manner. It consists of a cascade of flip-flops connected in series, forming a chain. The input data is applied to the first flip-flop in the chain, and as the clock pulses, the data propagates through the flip-flops, ultimately appearing at the output.

The logic circuit provided below demonstrates a serial-in serial-out (SISO) shift register. It comprises four D flip-flops that are interconnected in a sequential manner. These flip-flops operate synchronously with one another, as they all receive the same clock signal.



![Screenshot 2024-12-18 212335](https://github.com/user-attachments/assets/06826562-9ef9-4855-8277-0b3b40fd9f7b)

Figure 01 4 Bit SISO Register

The synchronous nature of the flip-flops ensures that the shifting of data occurs in a coordinated manner. When the clock signal rises, the input data is sampled and stored in the first flip-flop. On subsequent clock pulses, the stored data propagates through the flip-flops, moving from one flip-flop to the next.
Each D flip-flop in the circuit has a Data (D) input, a Clock (CLK) input, and an output (Q). The D input represents the data to be loaded into the flip-flop, while the CLK input is connected to the common clock signal. The output (Q) of each flip-flop is connected to the D input of the next flip-flop, forming a cascade.

**Procedure**



**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming.

Developed by:Sarankumar.V RegisterNumber:24010668
```
module EXP10(clk, sin, q);

input clk;

input sing

output [3:0] q;

reg [3:0] q;

always @(posedge clk)

begin

q[0] <= sin;

q[1] <= q[0];

q[2] <= q[1];

q[3] <= q[2];

end

endmodule
```

**RTL LOGIC FOR SISO Shift Register**

![Screenshot 2024-12-18 212354](https://github.com/user-attachments/assets/5814422c-b797-45f3-bb4d-bb1c744af484)

**TIMING DIGRAMS FOR SISO Shift Register**

![Screenshot 2024-12-18 212407](https://github.com/user-attachments/assets/331ef67e-e588-4514-a719-792240f85cb7)

**RESULTS**
Thus,SISO Shift Register using verilog and validating their functionality using their functional tables has successful execution of the program.
