# Multiprogramming Operating System Simulation - Phase 2

## **Project Overview**
Phase 2 of the project focuses on extending the system with **error handling**, **dynamic memory management**, and **page table generation** to simulate virtual memory functionality. This phase introduces the concept of handling **page faults** and managing jobs dynamically to improve the operating system's efficiency.

---

## **Phase 2 Features**

### **1. Error Handling**
- **Time Limit Exceeded (TLE)**:
  - Simulates scenarios where a job exceeds the predefined execution time.
- **Line Limit Exceeded (LLE)**:
  - Handles errors when a job writes or reads beyond the allocated memory line.
- **Page Faults**:
  - Identifies when the required data is not present in memory and initiates appropriate handling to retrieve it.

---

### **2. Dynamic Memory Management**
- **Page Table Generation**:
  - Randomly generates page numbers and assigns them to memory blocks.
  - Ensures each job gets a unique allocation of memory blocks.
- **Job Assignment**:
  - Dynamically assigns page numbers for each instruction within a job.
  - Adjusts page table size based on the number of active jobs and memory availability.

---

### **3. Workflow Steps**
1. **Generate Random Page Numbers**:
   - Assign random page numbers to jobs and map them in the page table.
   - Example: If a random number is 6, a specific block in memory is allocated.
   
2. **Handle Page Faults**:
   - If a required page is not in memory:
     - Search the page table for its location.
     - If not found, retrieve the data from secondary storage and update the page table.

3. **Job Execution**:
   - For each instruction in a job:
     - Fetch the corresponding page from memory.
     - If unavailable, handle it as a page fault.

4. **Repeat for All Jobs**:
   - Continue assigning random numbers and updating the page table until all jobs are executed.

---

## **Example Execution**
- **Job 1**:
  - Page Table: Randomly assigns pages (e.g., 30, 31, 32...).
  - Executes instructions and dynamically adjusts the page table.
  
- **Job 2**:
  - Similar random assignment and execution process.
  - Handles page faults and memory reallocation.

---

## **Technical Details**
- **Error Handling**:
  - TLE and LLE errors are detected and logged during job execution.
- **Dynamic Memory**:
  - Memory is segmented into pages and managed dynamically using a page table.
- **Page Fault Handling**:
  - Retrieves missing pages from secondary storage and updates the page table.

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
