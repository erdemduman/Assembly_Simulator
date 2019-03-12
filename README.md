# Assembly Simulator

## Instructions
#### Move Instructions
MOV reg, address <br />
MOV address, reg <br />
MOV reg, reg <br />
MOV reg, constant <br />
MOV address, constant <br /> <br />
For example MOV R1, #45 copies the value of register 1 to memory location 45. <br />

#### Addition and Subtraction Insructions
ADD reg, reg <br />
ADD reg, constant <br />
ADD reg, address <br />
SUB reg, reg <br />
SUB reg, constant <br />
SUB reg, address <br /> <br />
For example, ADD R1, R2 adds the value of register 2 to register 1. <br />

#### Print Instructions
PRN reg <br />
PRN constant <br />
PRN address <br /> <br />
For example, PRN #56 will print the value of the memory loacation 56 to the screen. <br />

#### Jump Instructions
JMP reg, lineAdress <br />
JMP lineAddress <br />
JPN reg, lineAdress <br /> <br />
For example, JMP R1, 32 jumps to line 32 of the program if the value of R1 is zero. JMP 23 jumps to
line 23 directly. <br />
JPN R1, 32 jumps to line 32 of the program if the value of R1 is zero or smaller. <br />

#### Other Instructions
HLT <br />
Halts the program and prints on the screen the contents of all registers as well as the the memory. <br />

## How to Compile & Run
Run makefile to compile the code. <br />
The format for the command line parameters is as follows: <br /> <br />
./sim 'filename' 'option' <br /> <br />

Option number can be the values below: <br />
• if option is 0, program will run and finish by executing each instruction.<br />
• if option is 1, program will execute each instruction after displaying the instruction first.
It also will print the contents of all the registers.<br />
• If option is 2, program will execute each instruction just like the option 1. This option
will also print the contents of the memory after each intruction execution. <br />
