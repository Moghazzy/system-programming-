Introduction to modi-SIC
The modi-SIC consists of
1. Same instructions set (Format 3) of SIC
2. Same idea of reservation of variables in memory using BYTE, WORD, RESB, RESW

modi-SIC is extened to include
1. Format 1 instuctions
2. Immediate Instruction (Format 3) that deals with an immediate value passed to as integer.
For the sack of simplification a list of modi-SIC instructions is attached at the end of project
description that have all instructions handled by modi-SIC + a full description of a new introduced
bit that states if the instruction is dealing with immediate or not.
modi-SIC implementation details
It takes as an input a text file (in.txt) that contains an assembly program written in modi-SIC
assembly language containing comments, number lines as shown in figure 1. The modi-SIC
assemble will be modified to accept also Format 1 instruction of SIC/XE. So this case must be
handled.
Generating Intermediate File
You will have to read the input file (with line numbers and comments) and generate an intermediate
file by removing the comments, number lines and keep only assembly instruction. This intermediate
file should be saved as (intermediate.txt).
Pass 1
Pass 1 should read the intermediate file and produce: Location Counter for all program lines
followed by the generation of the symbol table
The program should produce as output:
• (out_pass1.txt) that contains the corresponding location counter of the input Program
• (symbTable.txt) that contains the symbol table output of the input program
Pass 2
Pass 2 should read the intermediate file and produce: object code for all program lines followed by
the generation of the HTE record
The program should produce as output:
• (out_pass2.txt) that contains the corresponding object code of the input program
• (HTE.txt) that contains the corresponding object code of the input program in HTE format.
sic mod
