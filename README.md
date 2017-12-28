# Basic-OS
# Prerequisites NASM and QEMU

NASM is assembler which converts assembly language into raw machine code

QEMU is PC Emulator

# How does an OS work?

1.	When you ‘turn ON’ PC, microprocessor passes control to BIOS program which is always located at the same place on EPROM.
BIOS – BIOS is an integral part of your computer. It stands for Basic Input Output System. It is a program accessible to the microprocessor on an EPROM chip.
2.	When BIOS boots up (startup) your computer, it firsts determine whether all of the attachments are in place and operational. BIOS makes sure all the other chips, hard drives, ports and CPU function together.
3.	Once BIOS has found a bootable device, it copies the contents of device sector into RAM starting from physical address 0x7c00.
Or you can say BIOS loads contents of bootable device sector into RAM .
In computer disk storage, a sector is a subdivision of a track on a magnetic disk or optical disc. Each sector stores a fixed amount of user-accessible data.
4.	Once code has loaded to the address, it jumps to the address and executes the loaded code. This code is bootloader.
5.	Eg. of GRUB (GNU project) Grand Unified Bootloader – GNU GRUB is bootloader that allows user the choice to boot one of the multiple OS installed on a computer OR select a specific kernel configuration available on particular OS partition.
6.	Bootloader then loads the kernel at physical address 0x100000. This address is used as the start address for all big kernels.
7.	Kernel is the core of an OS. A kernel is the central part of an operating system. It manages the operations of the computer and the hardware. It is responsible for assigning and unassigning memory space which allows software to run.

