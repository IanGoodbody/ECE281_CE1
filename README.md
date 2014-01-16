ECE281_CE1
==========

### Abstract

Computer simulation of complex digital circuits gives the designer a high degree of flexability and
consistancy in modeling such digital systems, and understanding how to utilize these powerful tools
is key to the Electrical Engineering dicipline. This lab was used as an introduction to using VHDL
(VHSID Hardware Description Language) to model digital circuits. A simple digital logic circuit was
simulated and tested in the software to provide a proof of concept.

### Lab Set Up

The schematic for the three-input, four-gate digital circuit that was simulated in VHDL is given below: 

![alt text](https://raw2.github.com/IanGoodbody/ECE281_CE1/master/Circuit.JPG "Digital Circuit Schematic")

The circuit was simulated using VHDL code in the Xilinx ISE Design Suite. The same software was later
used to simulate and record the output of the circuit (signal F) for all combinations of the three 
inputs (signals A, B, and C).

### Lab Results and Analysis

The above diagram was used to produce the following boolean equation:

    *AB' + BC = F*
    
and the corresponding truth table:

    | A | B | C || F |
    |:-:|:-:|:-:||:-:|
    | 0 | 0 | 0 || 0 |
    | 0 | 0 | 1 || 0 |
    | 0 | 1 | 0 || 0 |
    | 0 | 1 | 1 || 1 |
    | 1 | 0 | 0 || 1 |
    | 1 | 0 | 1 || 1 |
    | 1 | 1 | 0 || 0 |
    | 1 | 1 | 1 || 1 |
    
This equation and truth tables were modeled in the two VDHL files provided. The input signals
were changed every 100 ns in decending order on the above truth table, 1 representing a HIGH
signal and 0 representing LOW. The output values, shown in the bottom row of the truth table,
corresponded with those in the truth table. 

![alt text](https://raw2.github.com/IanGoodbody/ECE281_CE1/master/Signal.JPG "Digital Signals")

