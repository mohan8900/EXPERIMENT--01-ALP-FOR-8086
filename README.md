## EXPERIMENT--01-ALP-FOR-8086
Name : A K MOHAN RAJ

Roll no : 212221230064
## Aim: 
To Write and execute ALP on fundamental arithmetic and logical operations

## Components required: 
8086  emulator 

## Theory :

Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.



 ## Running the Emulator :
 
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory

2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color .

3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 

5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 

7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,

8.	![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)


9.	Click on emulate to start emulation 

![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)

10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 

![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)

## Programs for arithmetic  operations

## Addition  of 8 bit ALP 

name "ADDITION"
org 100h
MOV AH,05H;
MOV BH,02H;
ADD AH,BH;
MOV CH,AH;
MOV AH,0H; 
MOV BH,0H;
HLT;


## Output  
### AH and BH registers for ADDITION
![mc1](https://user-images.githubusercontent.com/94154683/189403970-96ba85d7-0179-48bc-91de-e1d4fa33d4f5.jpeg)
### Performing 8 Bit ADDITION
![mc2](https://user-images.githubusercontent.com/94154683/189403964-fdea6abc-95d5-4cd0-b56b-1ab0297f45c5.jpeg)
### Moving to CH register
![mc3](https://user-images.githubusercontent.com/94154683/189403952-c619ed22-a9aa-4e50-ba80-2e53ea29cd18.jpeg)
### Resetting AH,BH register and Execution
![mc4](https://user-images.githubusercontent.com/94154683/189404217-18be4c6e-4133-4d48-ba71-3a686c0e03a1.jpeg)
### Flags:
![mcc](https://user-images.githubusercontent.com/94154683/189404757-b2c0bfed-23ec-4894-9c25-479445c9d934.jpeg)

## Subtraction   of 8 bit numbers  ALP 

name "SUBTRACTION"
org 700h
MOV AH,7H;
MOV BH,5H;
SUB AH,BH;
MOV CH,AH;
MOV AH,0H;
MOV BH,0h;
HLT;


## Output  
### AH and BH registers for SUBTRACTION
![mc21](https://user-images.githubusercontent.com/94154683/189404321-ba33c32e-c1f1-4957-b428-8632d2011110.jpeg)
### Performing 8 Bit SUBTRACTION
![mc22](https://user-images.githubusercontent.com/94154683/189404348-a83d7059-677b-45a1-93c4-b3670212817c.jpeg)
### Moving to CH register
![mc23](https://user-images.githubusercontent.com/94154683/189404378-59916647-d716-41d4-bf06-f80dc549b8af.jpeg)
### Resetting AH,BH register and Execution
![mc24](https://user-images.githubusercontent.com/94154683/189404416-4eec04b7-095d-44a0-af0c-08d0d09dea95.jpeg)
### Flags:
![mcc](https://user-images.githubusercontent.com/94154683/189404757-b2c0bfed-23ec-4894-9c25-479445c9d934.jpeg)


## Multiplication alp 

name "MULTIPLICATION"
org 700h
MOV AX,5H;
MOV BX,4H;
MUL BX;
MOV CX,AX;
MOV AX,0H;
MOV BX,0h;
HLT;

## Output  
### AX and BX registers for MULTIPLICATION
![mc31](https://user-images.githubusercontent.com/94154683/189404593-82040e4d-d826-4537-9631-c3c18c0d0a65.jpeg)
### Performing 8 Bit MULTIPLICATION
![mc32](https://user-images.githubusercontent.com/94154683/189404609-69996427-b408-4320-a122-157945cebfa1.jpeg)
### Moving to CX register
![mc33](https://user-images.githubusercontent.com/94154683/189404631-2577e6c0-a5ff-44ec-a2cd-4d0f24adc13f.jpeg)
### Resetting AX,BX register and Execution
![mc34](https://user-images.githubusercontent.com/94154683/189404659-e5e8c1fc-9223-4084-808a-0e8b4f61c956.jpeg)
### Flags:
![mcc](https://user-images.githubusercontent.com/94154683/189404757-b2c0bfed-23ec-4894-9c25-479445c9d934.jpeg)



## Division alp 

name "DIVISION"
org 700h
MOV AX,9H;
MOV BX,3H;
DIV BX;
MOV CX,AX;
MOV AX,0H;
MOV BX,0h;
HLT;

## Output  
### AX and BX registers for DIVISION
![mc41](https://user-images.githubusercontent.com/94154683/189405086-57e7e388-3b1c-4b08-9868-3d6533b19f5c.jpeg)
### Performing 8 Bit DIVISION
![mc42](https://user-images.githubusercontent.com/94154683/189405115-fb26c155-fc90-4578-8733-56c3c6818a8d.jpeg)
### Moving to CX register
![mc43](https://user-images.githubusercontent.com/94154683/189405131-c25a35d2-a788-4c2b-b3f2-af681bab8883.jpeg)
### Resetting AX,BX register and Execution
![mc44](https://user-images.githubusercontent.com/94154683/189405141-e296f15d-0e5c-4354-8bcd-987c033ab316.jpeg)
### Flags:
![mcc](https://user-images.githubusercontent.com/94154683/189404757-b2c0bfed-23ec-4894-9c25-479445c9d934.jpeg)

## Result :
Thus a program on ALP for the fundamental arithmetic and logical operations is done successful.

```



