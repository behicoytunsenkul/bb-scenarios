### 4- Environment Setups for Assembly Language
During our training, we need to install **NASM** so that we can code with assembly language on the terminal. However, unlike many programming languages, Assembly comes pre-installed on Linux.
To find out if NASM is installed on your system, enter the following command into the terminal:
```
whereis nasm
```
If you get ``nasm: /usr/bin/nasm`` output on the terminal screen after running the above command, it means nasm is installed on your system. However, if you only get ``nasm:`` output, it means that you do not have nasm installed on your system. To install nasm on your system, enter the following commands in order:
```
apt-get update
apt-get install nasm
```
After running the above commands, you can check whether the nasm installation has taken place with the ``whereis nasm`` command.
> After successful installation, let's start coding our **Hello World** application by proceeding to the next step.