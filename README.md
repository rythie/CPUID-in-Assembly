CPUID-in-Assembly
=================
This is only designed to run on x86 Linux machines.

How to Build from Source
------------------------
Where I have used 'nasm', 'yasm' could also be used.

### 32bit x86 machines
nasm -f elf cpuid.asm
ld -s -o cpuid cpuid.o

### 64bit x86 machines
nasm -f elf cpuid.asm
ld -s -m elf_i386 -o cpuid cpuid.o
