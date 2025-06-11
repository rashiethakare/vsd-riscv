# vsd-riscv
![Screenshot from 2025-05-20 19-55-35](https://github.com/user-attachments/assets/99ef65cd-b81f-45ef-9c3c-a189ce84cbf2)

![Screenshot from 2025-05-20 20-04-28](https://github.com/user-attachments/assets/d888aa40-5833-44de-a601-08719f5c5045)


![Screenshot from 2025-05-20 20-08-31](https://github.com/user-attachments/assets/e479996a-8b2b-4ac3-802d-de2ae389ee3f)


![Screenshot from 2025-05-20 20-10-04](https://github.com/user-attachments/assets/5c440252-e49a-4cdc-92d8-c7f5d64a59f6)


lab 2


![Screenshot from 2025-05-20 22-39-09](https://github.com/user-attachments/assets/6549838c-4114-49f6-a041-05e8d292b160)

![Screenshot from 2025-05-20 22-40-02](https://github.com/user-attachments/assets/7d03d55c-fec1-4219-9d9f-794a5de1378c)
![Screenshot from 2025-05-20 22-45-13](https://github.com/user-attachments/assets/6bafd87f-8598-4657-acd2-76d1aa70b1bc)
![Screenshot from 2025-05-20 22-46-02](https://github.com/user-attachments/assets/a55e7d5a-1248-4e45-9c16-79405f8b7c7d)


![Screenshot from 2025-05-20 22-59-59](https://github.com/user-attachments/assets/39c9937b-6fa4-486e-8113-d8a4136065b7)


![Screenshot from 2025-05-20 23-03-06](https://github.com/user-attachments/assets/c8be941a-d400-45e2-bbb1-a49b355a4e09)

![Screenshot from 2025-05-20 23-06-09](https://github.com/user-attachments/assets/dae6ac1d-0313-48fe-b36a-24921f25a432)

lab 3 spike 
![Screenshot from 2025-05-24 20-50-03](https://github.com/user-attachments/assets/856b5c3e-cc31-4555-a5cd-0c76938813d6)


![Screenshot from 2025-05-24 20-10-32](https://github.com/user-attachments/assets/84e9c979-bf0e-4664-beab-b05bdfc97ed0)
![Screenshot from 2025-05-24 20-37-58](https://github.com/user-attachments/assets/074c37f6-a633-42bd-b845-e5db42254865)


1. RISC-V (pronounced "risk-five") is a modern instruction set architecture (ISA) developed originally to support computer architecture research and education.
It is an open-standard ISA, meaning it is free to use and implement by anyone without licensing fees.
Designed with simplicity and modularity in mind, RISC-V allows for:
 • Custom extensions tailored to specific applications.
 • Easier optimization for different domains (e.g., embedded systems, high-performance computing).
RISC-V follows the principles of Reduced Instruction Set Computing (RISC):
 • Focuses on a smaller number of simple instructions.
 • Simplifies hardware design, which can lead to improved performance and efficiency.
2.	RV32I Base Integer Instruction Set
The RV32I Base Integer Instruction Set is a fundamental subset of the RISC-V instruction set architecture (ISA) designed for 32-bit integer operations. It provides the essential instructions needed to perform basic computing tasks. Here’s a detailed breakdown:
Overview of RV32I:
•	32-bit Architecture: The "32" in RV32I refers to the 32-bit width of the instruction set, indicating that instructions and data are processed as 32-bit entities.
•	Base Integer Instructions: The "I" stands for "Integer," meaning this set covers the basic operations for integer arithmetic, logic, and data manipulation.
Basic Operations:
•	Arithmetic: Add, subtract, multiply, divide.
•	Logical: AND, OR, XOR, shift operations.
•	Data Movement: Load from memory, store to memory.
•	Control Flow: Conditional branches, jumps, subroutine calls.
 
Instruction Formats:
•	R-Type: For register-to-register operations (e.g., add, sub).
•	I-Type: For immediate value operations and loads (e.g., addi, lw).
•	S-Type: For store operations (e.g., sw).
•	B-Type: For branch operations (e.g., beq).
•	U-Type: For upper immediate operations (e.g., lui).
•	J-Type: For jump operations (e.g., jal).

Instruction Set 
![image](https://github.com/user-attachments/assets/ce569a07-a3b9-41d0-a4d1-7308a24127fb)

32 bit risc-v instruction set 

![image](https://github.com/user-attachments/assets/a77cd61d-7e47-40a2-8c32-02e4d2861545)


3.	BASE INSTRUCTION FORMATS AND TYPES
	In RISC-V, Generally in base RV32I ISA, there are four core instruction formats (R/I/S/U)
  There are a further two variants of the instruction formats (B/J) based on the handling of immediates, these base instruction formats that define how instructions are encoded within a 32-bit word
  Finally, it can be classified as,
•	R-type: Register-Register operations
•	I-type: Immediate operations
•	S-type: Store operations
•	B-type: Branch operations
•	U-type: Upper immediate operations
•	J-type: Jump operations
a) R-TYPE: REGISTER-REGISTER OPERATIONS
  Purpose: Performs operations using an immediate (constant) value and a register.

![image](https://github.com/user-attachments/assets/98143392-67c2-462b-8a63-0bd29df41dd0)

  Fields:
•	opcode: Specifies the type of instruction.
•	rd: Destination register.
•	funct3: Further specifies the operation.
•	rs1: Source register.
•	imm[11:0]: 12-bit immediate value.

b) I-TYPE: IMMEDIATE OPERATIONS
	Purpose: Performs operations using an immediate (constant) value and a register.
 
 ![image](https://github.com/user-attachments/assets/d7724f9c-4f4e-49f0-9773-afae156407ed)

  Fields:
•	opcode: Specifies the type of instruction.
•	rd: Destination register.
•	funct3: Further specifies the operation.
•	rs1: Source register.
•	imm[11:0]: 12-bit immediate value.
S-TYPE: STORE OPERATIONS
  Purpose: Stores data from a register to memory.
  
![image](https://github.com/user-attachments/assets/b1483f5c-e53c-4426-9f84-d135eba9ebef)

  Fields:
•	opcode: Specifies the type of instruction.
•	imm[11:5]: Higher bits of the 12-bit immediate value.
•	funct3: Further specifies the operation.
•	rs1: Base address register. 
•	rs2: Source register.
•	imm[4:0]: Lower bits of the 12-bit immediate value.

c) B-TYPE: BRANCH OPERATIONS
	Purpose:	Performs	conditional	branches	based	on	the comparison of two registers.
 
![image](https://github.com/user-attachments/assets/5b132673-c25c-43c0-8ecd-c3ec2e1a4569)

 Fields:
•	opcode: Specifies the type of instruction.
•	imm[12]: Sign bit of the immediate value.
•	imm[10:5]: Higher bits of the immediate value.
•	funct3: Further specifies the operation.
•	rs1: First source register.
•	rs2: Second source register.
•	imm[4:1]: Lower bits of the immediate value.
•	imm[11]: Middle bit of the immediate value.

d) U-TYPE: UPPER IMMEDIATE OPERATIONS
  Purpose: Loads a 20-bit immediate value into the upper 20 bits of a register.
  
  ![image](https://github.com/user-attachments/assets/8aebc8ef-f80b-453a-9d4e-518bd7b1efda)

  Fields:
•	opcode: Specifies the type of instruction.
•	rd: Destination register.
•	imm[31:12]: 20-bit immediate value.

e) J-TYPE: JUMP OPERATIONS
	Purpose: Performs jumps to a target address specified by an immediate value.
 
![image](https://github.com/user-attachments/assets/bfe65d0b-ed42-4e27-aec4-f07a6ca4df29) 

  Fields:
•	opcode: Specifies the type of instruction.
•	rd: Destination register.
•	imm[20]: Sign bit of the immediate value.
•	imm[10:1]: Lower bits of the immediate value.
•	imm[11]: Middle bit of the immediate value.
•	imm[19:12]: Higher bits of the immediate value.

![image](https://github.com/user-attachments/assets/9cbbb86a-4c89-455c-a78e-513e23a943a1)

lab 4 
task 4

![Screenshot from 2025-06-02 20-07-11](https://github.com/user-attachments/assets/06e7fe00-3f49-49a7-93b9-c6ecfc9a1a45)
1.ADD r6, r2, r1
![Screenshot from 2025-06-02 20-53-16](https://github.com/user-attachments/assets/38166580-924b-4ee0-af83-9158554e8989)

2.SUB r7, r1, r2
![Screenshot from 2025-06-02 21-48-13](https://github.com/user-attachments/assets/fd808ff2-5ec2-414f-865e-580d52a823f7)

3.AND r8, r1, r3
![Screenshot from 2025-06-02 21-48-22](https://github.com/user-attachments/assets/ba86518e-735b-42e9-9976-7f61943e05c8)

4.OR r9, r2, r5
![Screenshot from 2025-06-02 21-48-30](https://github.com/user-attachments/assets/c77b2d56-8169-4d1e-b052-3e0a692c9731)

5.XOR r10, r1, r4
![Screenshot from 2025-06-02 21-48-42](https://github.com/user-attachments/assets/a193a3f0-e6a4-410c-8d3b-57d42ebeb725)

6.SLT r11, r2, r4
![Screenshot from 2025-06-02 21-48-53](https://github.com/user-attachments/assets/78eef2bd-644d-4604-a0ae-f225fc490666)

7.ADDI r12, r4, 5
![Screenshot from 2025-06-02 21-49-47](https://github.com/user-attachments/assets/e9029310-053c-4091-a723-a8b54332ddbd)

8.SW r3, r1, 2
![Screenshot from 2025-06-02 21-50-12](https://github.com/user-attachments/assets/a21c55de-37ce-445f-a048-1153261ad3ad)

9.LW r13, r1, 2
![Screenshot from 2025-06-02 21-51-36](https://github.com/user-attachments/assets/bd4cd370-6959-46ca-9809-970e9e03ae38)

10.BEQ r0, r0, 15

![Screenshot from 2025-06-02 21-51-48](https://github.com/user-attachments/assets/848ba19f-3195-4fed-9f02-c353bcf7ed16)

task 5
#Implementing Full Adder using VSDSquadron Mini









