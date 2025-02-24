Download Link :https://programming.engineering/product/csu22022-project-2-microcoded-instruction-set-processor/


# CSU22022-Project-2-MICROCODED-INSTRUCTION-SET-PROCESSOR
CSU22022 Project 2 MICROCODED INSTRUCTION SET PROCESSOR
Description:

The second project will implement a Microprogrammed Instruction Set Processor.

This builds on the VHDL model from the first project.

The following modifications are required:

Increase the number of registers in the register-file from 32 to 33.

This requires an additional select bit for the two multiplexers (Bus A and Bus

B) and the destination decoder. These are separate signals (TD, TA, TB) from

the Control Memory. See Figure 1. The size of the registers in the register-file

is 32 bits.


Consequently all components of the Datapath (e.g. MUXs in the register-file,

decoder in the Register file, Arithmetic/logic Unit, Shifter and MUXs) are 32 bit

operations.


Add and test Memory M (512 x 32) and Control Memory (256 x 41) to your

project. MUX M will feed 32 bit addresses from ether the Bus A or the PC into

the Memory M but only the 9 least significant address bits will be used to

index into the array. This restricts the memory size to 512. Furthermore, the

CAR feeds 17 bit addresses into the the Control Memory but only the 8 least

significant address will be used to select a memory location in the Control

Memory.

Implement all the components shown in Figure 1 on page 3.

Design reset logic for PC and CAR registers. This will enable you to start your

program.


Write microprogramms for the Control Memory that implement the following

instructions:

o ADI, LD, SR, INC, NOT, ADD, unconditional jump, and conditional

branch (only one condition).

Write machine code for the Memory M that demonstrates the use of the

following instructions:

o ADI, LD, SR, INC, NOT, ADD, unconditional jump, and conditional

branch (only one condition).

The Microprogmmmed Instruction Set Processor block diagram is shown in

Figure 1 on page 3. Figure 1 is based on Figure 8-26 in Mano and Kime [2] but was

modified to suit the assignment.

The Functional Unit should have the functionality defined in the Table 1 on

page 2.

Discuss your simulation results. The CSU22022 lecture notes provide the

necessary information to complete the project.

If the entire project is working (you must demonstrate that you can execute the

following instructions: ADI, LD, SR, INC, NOT, ADD, unconditional jump, and

conditional branch (only one condition)), you can gain additional 20% by

implementing a carry-lookahead adder (CLA).

DUE: Tuesday, 5thJanuary 2021

Please submit your VHDL‐code and test‐benches including all simulation results

to Blackboard.
