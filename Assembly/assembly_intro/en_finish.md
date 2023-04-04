### 6- Let's Run Our App
Now that we have examined all the commands we wrote in our **hello.asm** file, we can move on to the step of running our application.
First, let's enter the following command on our terminal screen:
```
nasm -f elf64 -o hello.o hello.asm
```
The above command tells Netwide Assembler (NASM) to create a 64-bit ELF object file from the assembly code in "hello.asm".
```
ld -o hello hello.o
```
This command uses the GNU linker (ld) to generate an executable named "hello" from the object file "hello.o".
Now that we have completed all the steps to get our application working, let's run our application using the following command:
```
./hello
```
After running this command, our application file will be compiled and output ``Hello World`` to the terminal screen.

> CONGRATULATIONS. You have successfully completed our assembly language introductory training.