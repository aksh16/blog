---
title: "Assembly_basics"
date: 2023-05-24T20:01:01-07:00
draft: False
---
Why would you care about assembly? Well ideally you won't.\
A typical programmer today works mostly with a high level programming language that is so far away from actual CPU instructions and low level memory (What is low level memory? Keep reading and you will find out) that the compiler and the OS work out the details without the programmer having to worry about it.
That is how most businesses would want to people to work. Writing assembly is time consuming. Programmers being able to churn out as much code in as little time as possible is beneficial to companies. More code means more features and more features mean more business and ultimately more money, higher market share, happier shareholder etc. You get what I am saying.

But some of us our curious as to what happens underneath the hood. Just as a C compiler understand C, JVM understands Java, Assemblers understands assembly and then output machine code. Now assembly is not a specific language per se, more like a template that most CPU manufacturers follow. Intel's assembly's syntax is different from AT&T's syntax these are part of the CISC architecture. RISC architectures such MIPS have some what similar syntax but fewer instructions. RISC and CISC are topics for a different blog. Now that I have bored you in setting up the stage, lets get down to what is important.

## Registers
These are actual physical locations inside a CPU. They can be accessed really quickly. Size of a register is typically 64 bit in most modern machines. And the word size is in most cases equal to the register's size. And word is size of data that a CPU can process in one cycle.

## Memory
RAM (Random Access Memory) is typically referred to as memory. It is larger in size compared to registers. There might be 64 registers each with 8 bytes of memory whereas the same machine can have 4 GB of memory. Access to memory is slower and can be thought of as one long array which can be accessed by its indices.

## Instructions
### mov
It is more like copy than actually moving values.\
You can move values between registers or between registers and memory.
