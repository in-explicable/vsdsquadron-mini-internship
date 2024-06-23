#  VSDSquadron Internship 2024

The program is based on the RISC-V architecture and uses open-source tools to teach people about VLSI chip design and RISC-V. The instructor for this internship is Kunal Ghosh Sir.

##  Basic Details

**Name:** Nivesh S  
**College:** Puducherry Technological University  
**Email ID:** niveshsr@gmail.com 

**GitHub Profile:** [in-explicable](https://github.com/in-explicale)  
**LinkedIn Profile:** [nivesh-s](https://www.linkedin.com/in/nivesh-s)

----------------------------------------------------------------------------------------------------------------

<details>
<summary><b>Task 1:</b> Create GitHub repo. Install RISC-V toolchain using VDI shared. Refer to C based Lab video and RISC-V based lab videos. Upload snapshot of compiled C code and RISC-V Objdmp on the GitHub repo</summary>   
<br>

 **1.Installation**<br />
  After installing the tools then open the terminal on Ubuntu to type the command.<br />
  ![Installing Ubuntu   VMBox](https://github.com/VijayN53/VSDSquadron_Mini_Internship/assets/106604062/51924514-846f-4fe7-8d96-2619dad511f0)

  
  **2.Command for Installing Leafpad**<br />
  ```
  $ sudo apt install leafpad
  ```
  
  **3.Command for Opening Leafpad**<br />
  ```
  $ cd
  $ leafpad filename.c &
  ```
  ![Sample_C_code](https://github.com/VijayN53/VSDSquadron_Mini_Internship/assets/106604062/584b7959-1760-4e50-bb75-fd011370cb2b)

  
  **4.Command for Compiling the Output**<br />
  ```
  $ gcc filename.c
  $ ./a.out
  ```
  ![Output of Sample code](https://github.com/VijayN53/VSDSquadron_Mini_Internship/assets/106604062/b1e1a5dc-295e-4c80-b871-5c5154056b9f)
    
  **5.Command for Compiling the Code using RISCV Compiler**<br />
  ```
  $ riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o filename.o filename.c
  $ ls -ltr filename.o
  ```
  ![Installing RISC Compiler](https://github.com/VijayN53/VSDSquadron_Mini_Internship/assets/106604062/d925b284-359e-444e-a7bb-62dd9a135d06)

  **6.Command to View the Assembly Code**<br />
  ```
  $ riscv64-unknown-elf-objdump -d filename.o 
  $ riscv64-unknown-elf-objdump -d filename.o | less 
  /main //to view the main function of the code
  ```
  ![Main Function Assembly code](https://github.com/VijayN53/VSDSquadron_Mini_Internship/assets/106604062/e3323abe-ece5-481a-8c1a-70e1b5c26ada)
    
  **7. Command to View the Assembly Code**<br />
  ```
  $ riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o filename.o filename.c
  $ riscv64-unknown-elf-objdump -d filename.o | less 
  /main 
  ```
  ![Assembly code for ofast command](https://github.com/VijayN53/VSDSquadron_Mini_Internship/assets/106604062/1e14ee97-c3ae-4644-80fa-bed8a9dbefb2)
 *** 
