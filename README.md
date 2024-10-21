# MOS Multiprogramming Operating System

This project implements a **Multiprogramming Operating System (MOS)** in three phases, gradually adding complexity and functionality. It simulates how jobs are handled by the system, including input/output management, error handling, and memory paging. Each phase builds upon the previous one, starting with basic execution and moving toward more advanced features like multiprogramming.

## Table of Contents
- [Project Overview](#project-overview)
- [Phase 1](#phase-1)
- [Phase 2](#phase-2)
- [Phase 3](#phase-3)
- [Installation](#installation)
- [Usage](#usage)
- [Contributors](#contributors)

## Project Overview

This project simulates an **Operating System** that evolves over three phases, each improving the system's ability to handle multiple jobs and manage resources. The project is built in a modular manner, allowing you to see how the system grows from simple, single-job execution to a robust multiprogramming environment.

## Phase 1

**Phase 1** represents the simplest form of MOS, focused on executing a single job at a time without any multiprogramming features. The goal of this phase is to establish the foundational functions of the system:

### Key Features:
- **Single Job Execution**: Only one job is loaded and executed at a time.
- **Job Input (Card Reader)**: Jobs are loaded from the **Card Reader** into **Main Memory** starting at address `00`.
- **Instruction Execution**: The **CPU** fetches and executes instructions in sequence, including **Load**, **Store**, **Compare**, and **Branch**.
- **Interrupt Handling (SI)**:
  - **SI = 1**: **Read** from the Card Reader.
  - **SI = 2**: **Write** to the Line Printer.
  - **SI = 3**: **Terminate** the job after completion.
- **Job Completion**: Once the job is finished, the system clears memory and resets for the next job.

This phase provides a basic **fetch-execute** cycle without multitasking or error handling.

## Phase 2

**Phase 2** introduces more advanced features like multiprogramming, error handling, and memory management. It builds upon Phase 1 by adding significant capabilities:

### Key Features:
- **Basic Multiprogramming**: The system now supports loading and managing multiple jobs concurrently.
- **Paging Mechanism**: Memory is managed using paging with a **Page Table Register (PTR)** for efficient memory access and protection.
- **Advanced Interrupt Handling**:
  - **PI (Program Interrupts)**: Handles errors such as invalid operations.
  - **TI (Timer Interrupts)**: Enforces time limits to ensure jobs don’t overrun.
  - **SI (Service Interrupts)**: Manages input/output, similar to Phase 1.
- **Error Handling**: Includes mechanisms to manage system errors and job failures.

This phase introduces more sophisticated memory and job management, allowing the system to be more efficient and stable.

## Phase 3

Phase 3 continues to build on the system's capabilities with more complex scheduling, resource allocation, and protection mechanisms (if applicable). More details can be provided once this phase is implemented.

## Installation

To run the MOS project locally, follow these steps:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/Swapnilpatil03/Assignment_intern.git
    ```

2. **Navigate to the Project Directory**:
    ```bash
    cd Assignment_intern
    ```

3. **Run the Program**:
    Instructions for running the different phases of the system will be added here.

## Usage

- **Phase 1**: Demonstrates how a single job is executed in the MOS environment with basic I/O handling.
- **Phase 2**: Shows multiprogramming and error handling in action.
- More detailed usage instructions for each phase will be added as the project progresses.



