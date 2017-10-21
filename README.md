# CrazySmallCPU
This repository holds the files associated with Warren's crazy small
breadboard CPU built with only ten chips. For more details on the design of
the CPU itself, see the
[Crazy Small CPU website.](http://minnie.tuhs.org/Programs/CrazySmallCPU)

The files are:
 * _crazycpu.circ_, a version of the CPU that runs in Logisim
 * _output.pdf_, a PDF version of the CPU's breadboard design done in Kicad
 * _cas_, the assembler for the CPU
 * _clc_, a very crude compiler that outputs assembly that can be given to _cas_
 * _csim_, a simulator that can run assembled programs. This allows you to test programs without loading them into Logisim or burning ROMs
 * _gen_alu_, a program to generate the contents of the ALU ROM
 * _notes_, my journal and notes as I went through the design and implementation stages
 * _Makefile_, to help make some of the ROM files. _make all_ will build the ALU ROM contents, assemble _fibminsky.s_ and produce the top and bottom control ROM images

Some example programs include:
 * _fibminsky.s_, a program that calculates Fibonacci numbers and then draws a sine wave using Minsky's circle algorithm
 * _genfibn_, a Perl program that generates the assembly code for the Fibonacci program. You tell it what size Fibonacci number to generate, up to 27 digits
 * _minsky.cl_. This is a reimplementation of the Minsky's circle algorithm program in the high-level language, just to test the compiler
 
 If you want to leave any comments, feel free to use the [GitHub issues page](https://github.com/DoctorWkt/CrazySmallCPU/issues) for this purpose.
