# As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.
# Veriog code is being executed and the waveforms are generated using the gtkwave

# Aim: To verify the Functional Simulation:-
# Table of contents
- [1.RISC-V RV32I](#1-RISC-V-RV32I)
 - [2.BLOCK DIAGRAM OF RISC-V RV32I](#2-BLOCK-DIAGRAM-OF-RISC-V-RV32I)
 - [3.INSTRUCTION SET OF RISC-V RV32I](#3-INSTRUCTION-SET-OF-RISC-V-RV32I)
 - [4.FUNCTIONAL SIMULATION](#4-FUNCTIONAL-SIMULATION)
    - [4.1 About iverilog and gtkwave](#41-About-iverilog-and-gtkwave)
    - [4.2 Installing iverilog and gtkwave](#42-Installing-iverilog-and-gtkwave)
    - [4.3 The output waveform](#43-The-output-waveform)
  
   ## 1. RISC-V RV32I

This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.

## 2. BLOCK DIAGRAM OF RISC-V RV32I
![Screenshot 2024-03-04 212106](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/1a853fae-88e7-452d-a264-ae84514dfbcd)

3. INSTRUCTION SET OF RISC-V RV32I

![Screenshot 2024-03-04 212158](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/2aa5df6b-de5f-4b6c-857e-08599757d7df)


![Screenshot 2024-03-04 212226](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/09aa697b-0be3-4833-b835-ac2bb117c545)
## 4. FUNCTIONAL SIMULATION

### 4.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.
  
### 4.2 Installing iverilog and gtkwave
- **For Ubuntu**
 Open your terminal and type the following to install iverilog and GTKWave
 ```
 $   sudo apt get update
 $   sudo apt get install iverilog gtkwave
 ```

![Screenshot 2024-03-04 215547](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/9dd74f3f-f328-41b7-a24b-6d334901153f)

- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**

 ```
 $ git clone https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/blob/main/README.md
 $ cd anushree
```


![Screenshot 2024-03-04 220801](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/bfff6c94-569b-47b6-aeef-3703a9fe69ae)

To simulate and run the Verilog code, enter the following commands in your terminal.


$ iverilog -o hello hello.v hello_tb.v

$ ./hello

![Screenshot 2024-03-04 221323](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/e1370bdb-d618-4dd3-a472-11439495ca37)

To see the output wave
orm in gtkwave, enter the following commands in your terminal.
$ gtkwave hello.vcd

![Screenshot 2024-03-04 222213](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/6221f17d-b43b-40ed-b60b-dfd14bfbf9ae)

![Screenshot 2024-03-04 222340](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/cf21b20e-fa24-483e-b070-1a3cecddf2d6)

4.3 The output waveform
The output waveform showing the instructions performed in a 5-stage pipelined architecture.

Instruction 1:add r6,r2,r1

![Screenshot 2024-03-04 212311](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/7ebe31b2-147b-4373-b249-9b5cee0448b4)

Instruction 2:sub r7,r1,r2

![Screenshot 2024-03-04 212333](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/c0ebb367-f175-4de7-90bd-726c6624379e)

Instruction 3:and r8,r1,r3

![Screenshot 2024-03-04 212426](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/2af62373-c173-4f0f-9779-16428cf14a2e)

Instruction 4:or r9,r2,r5

![Screenshot 2024-03-04 212616](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/35be3784-1039-4a2b-a570-efd70cb92974)

Instruction 5:xor r10,r1,r4

![Screenshot 2024-03-04 212714](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/7833df8d-20e2-4f83-971c-d2a0e66a5e18)

Instruction 6:slt r11,r2,r4

![Screenshot 2024-03-04 223234](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/da69ac4d-32c8-4c4c-b397-cf99da348069)

Instruction 7:addi r12,r4,5

![Screenshot 2024-03-04 223305](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/f30559af-d155-4939-839f-fe555e533002)

Instruction 8:sw r3,r1,2

![Screenshot 2024-03-04 223332](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/93e03cc6-0199-49da-9b93-60751951d752)

Instruction 9:lw r13,r1,2

![Screenshot 2024-03-04 223401](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/74e41223-e347-4053-813f-dde1dd5457f1)

Instruction 10:beq r0,r0,15

![Screenshot 2024-03-04 223428](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/ce1210a5-7f0c-4ef4-aaf6-b598ec67abbc)

After branching, performing Instruction 11:add r14,r2,r2

![Screenshot 2024-03-04 223513](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/1faec9d9-8117-4cbd-81bc-3eddf5a91fef)

Full 5-stage instruction pipeline and pc-increment description Waveform

![Screenshot 2024-03-04 223550](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/883b7dca-fc23-423d-b82e-ad57c198f603)

![Screenshot 2024-03-04 223626](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/3c32fb53-1228-4ed7-b266-0c2d665ff302)

![Screenshot 2024-03-04 223706](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/01032a0b-1a13-4176-bffa-9ace3c9c2a5e)











