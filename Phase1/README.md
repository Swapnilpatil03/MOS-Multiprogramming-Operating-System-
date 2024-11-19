# Multiprogramming Operating System Simulation - Phase 1

## **Project Overview**
This project is a simulation of a multiprogramming operating system, implemented in **C++**. It focuses on simulating the management of system resources, handling jobs, and ensuring efficient multitasking. Phase 1 lays the groundwork for the system by defining key functionalities like memory management, instruction handling, and input/output operations.

---

## **Phase 1 Features**

### **1. BIOS Simulation**
- **BIOS Initialization**: Simulates the booting process by invoking BIOS scripts.
- **Device Initialization**: Loads devices into the system.
- **RAM Partitioning**:
  - Divides memory into volatile and non-volatile regions.
  - Tracks total available RAM and allocates appropriate blocks for processes.

---

### **2. Instruction Processing**
- **Opcode Execution**:
  - Reads instructions with their opcode and operands.
  - Handles memory addressing for data fetching.
- **Instruction Types**:
  - **Read**: Retrieves data from memory.
  - **Write**: Transfers data to a specific memory location.
  - **Arithmetic Operations**: Simple operations based on loaded instructions.
  - **Branching and System Calls**: Implements conditional jumps and interrupts.

---

### **3. Memory Management**
- **Memory Blocks**:
  - Segments main memory into predefined blocks for process allocation.
  - Loads blocks into active RAM during execution.
- **Data Transfer**:
  - Moves instructions and data from input to memory locations.
  - Utilizes instruction registers for execution tracking.

---

## **Example Workflow**
1. **Initialize System**: The BIOS script initializes RAM and loads devices.
2. **Instruction Loading**:
   - Fetch instructions from input files.
   - Decode and store instructions in main memory blocks.
3. **Execution**:
   - Process instructions sequentially.
   - Handle system calls and exceptions during execution.
4. **Output**:
   - Generate results or errors based on execution outcomes.

---

## **Technical Details**
- **Languages Used**: C++.
- **Modules Implemented**:
  - BIOS simulation.
  - Memory segmentation and management.
  - Instruction handling.
- **Input/Output**:
  - Input: Set of instructions with opcodes and memory addresses.
  - Output: Execution trace, results, or error logs.

---

## **Usage Instructions**
1. Clone the repository:
   ```bash
   git clone https://github.com/Swapnilpatil03/MOS-Multiprogramming-Operating-System-.git

2. Navigate to the project directory
   ```bash
   cd MOS-Multiprogramming-Operating-System-

3. Compile the project:
   ```bash
   g++ -o MOS_simulation main.cpp

4. Run the executable:
   ```bash
   ./MOS_simulation


## Future Enhancements (Phase 2)
Implementation of virtual memory using segmentation.
Handling advanced system calls and interrupts.
Optimized multitasking and process scheduling.
