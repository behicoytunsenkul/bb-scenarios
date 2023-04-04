```
mov eax,4
mov ebx,1
mov ecx, msg
mov edx,13
int 0x80
```
This section contains the steps to print the text "Hello World" stored in the msg variable using the Linux system call. Now let's examine these steps:
* **mov eax,4** -> It records the syscall number eax for printing. 4 is the write system call number for the print operation.
* **mov ebx,1** -> The file descriptor to be used for printing to the screen. 1 is the file descriptor of the standard output file.
* **mov ecx,msg** -> ecx saves the memory address of the message to be printed.
* **mov edx,13** -> Specifies the number of bytes to print. 13 bytes is the number of characters in the "Hello World" string.
* **int 0x80** -> Triggers syscall and eax takes action based on recorded syscall number. In this case, the write system call is triggered because eax is registered and the message is printed.

```
mov eax,1
xor ebx
int 0x80
```
The last part of our code includes the steps to terminate the program. Let's examine these steps in order:
* **mov eax,1** -> eax records the system call number to be used to terminate the program. 1 is the exit syscall number.
* **xor ebx,ebx** -> Used to set exit code to 0. This indicates that the program terminated successfully.
* **int 0x80** -> Triggers the syscall and eax performs the operation based on the syscall number recorded.

> You can skip to the last step where we will learn how to run the first application we made in assembly language.