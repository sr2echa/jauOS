# jauOS

## Introduction

Welcome to `jauOS`, a rudimentary yet insightful operating system built from the ground up using Assembly and C. This project serves as a foray into the lower-level aspects of operating system development, featuring a monolithic kernel architecture. `jauOS` is an educational venture that demonstrates the core principles of OS design, offering a hands-on experience in system programming.

## Features

- **Monolithic Kernel**: A robust, single-tier architecture that integrates core functionalities within a single kernel space, enhancing efficiency and control.
- **Boot Process**: Customized bootloader written in Assembly, facilitating the initial system setup and transition from real mode to protected mode.
- **Memory Management**: Implements basic paging for memory management, showcasing the fundamental concepts of virtual memory and address translation.
- **Process Management**: Features process creation and management, including the implementation of the `fork()` system call, echoing the functionalities seen in UNIX-like systems.
- **Interrupt Handling**: Efficient management of hardware and software interrupts, including custom handlers for exceptions and a basic Interrupt Descriptor Table (IDT).
- **Console Interface**: A simple console for user interaction, capable of handling basic commands and interfacing with the kernel.
- **PS/2 Keyboard Driver**: Custom driver to handle keyboard inputs, translating keypresses into ASCII characters for processing.

## System Requirements

- **Processor**: Requires a CPU with support for the x86 architecture.
- **Memory**: Minimum of 64 MB RAM recommended for optimal performance.
- **Storage**: Requires minimal storage for the kernel and associated files along with the boot image.
- **A20 Line**: System must support enabling the A20 line for accessing extended memory.
- **Virtualization/Emulation Environment**: Compatible with virtualization tool - Bochs for testing and development purposes.

## Kernel Details

- **Type**: Monolithic architecture, encompassing all core components and drivers within a single kernel space.
- **Language**: The kernel core is written in C for modularity and maintainability, with critical segments in Assembly for direct hardware manipulation.
- **Bootloader**: Custom bootloader, initiating the kernel loading process and handling the switch from 16-bit real mode to 32-bit protected mode.

## Memory Management

- **Paging**: Implements a basic paging mechanism to handle memory management. This includes setting up page tables and managing memory allocation requests from processes.

## Process scheduling

- **Round-Robin Scheduling**: Incorporated a simple yet effective round-robin scheduling algorithm, demonstrating basic process scheduling and multitasking
