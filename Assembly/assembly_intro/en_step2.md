### 5- Let's Code Our First App
Before we start coding our application, we first need to set up the ``nano`` and ``touch`` feature to be able to perform file operations. Enter the following command to perform the installation on your system:
```
apk add build-base
apk add nano
apk add nasm
```
After the installation is complete, let's clear our terminal screen with the ``clear`` command. If we're ready, let's start coding our first app:
First, let's create our file where we will write our codes with the ``nano hello.asm`` command. Our file screen will appear.
Enter the following codes into your file:
```
section .data
     msg db "Hello World"i,0
section .text
     global _start
_start:
     mov eax,4
     mov ebx,1
     mov ecx, msg
     mov edx,13
     int 0x80
     mov eax,1
     xor ebx
     int 0x80
```
Before moving on to the step of running our code, let's examine what the above commands do one by one:
```
section .data
     msg db "Hello World",0
```
In this section, we have defined a variable named **msg**. The msg variable is defined as a string of bytes with the **db** command. The value 0 at the end indicates the end of the array.
```
section .text
     global _start
_start
```
In this section, the code part of the program is defined. The **_start** tag indicates the start of the program. The **global** tag makes it accessible externally.

> Proceed to the next step to review the commands in **_start**.