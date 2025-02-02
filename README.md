# 16-Bit-Processor-Indirect.logisim
# Need Statement:-

## "Design and simulate a 2-stage pipelined 16-bit processor which executes 3 address format code snippet using Indirect addressing mode"

# Brief description of the functional specifications of the Processor designed:

1. Processor Architecture:
- The processor consists of two pipeline stages: Instruction Fetch (IF) and Execution (EX).
- It operates on 16-bit data.

2. Instruction Set and Addressing Mode:
- The processor supports a 3-address format, meaning each instruction specifies three operands.
- Indirect addressing mode is employed, indicating that the operand's address is stored in a register or memory location, rather than being directly provided in the 
   instruction.

3. Registers:
- The processor includes a minimal set of registers, such as:
- General-purpose registers for storing operand addresses and intermediate results.
- A dedicated register for holding the indirect address reference.

4. Instruction Format:
- The instruction format is designed to accommodate the 3-address format and indirect addressing mode.
   Example format: OPCODE R1, R2, R3, where:
- OPCODE represents the operation code.
- R1, R2, and R3 are registers that may hold operands or indirect addresses pointing to actual operands in memory.

5. Pipeline Stages:
- Instruction Fetch (IF): Fetches the instruction from memory.
- Execution (EX): Executes the instruction, retrieving operand addresses from registers and performing the specified operation on the corresponding data.

6. Pipeline Hazard Handling:
- Address hazards need to be addressed to ensure the correct operand is available for execution.
- Possible solutions include stalling the pipeline or implementing forwarding mechanisms to resolve dependencies.

7. Memory Access:
- The processor interacts with memory to fetch and store data. In indirect addressing mode, a register holds the memory address where the actual operand is stored.
- The memory location pointed to by the register is accessed to retrieve the operand for execution.

8. Control Unit:
- The control unit manages the flow of instructions through the pipeline, controls the execution of operations, and handles data transfers.
- It resolves indirect addressing by accessing the memory location stored in the register before execution.

9. Simulation and Testing:
- The designed processor should be simulated using appropriate tools to validate its functionality.
- Test cases should be created to cover a range of instructions, addressing scenarios, and potential edge cases related to indirect addressing mode.

10. Performance Considerations:
- Evaluate the performance of the pipelined processor, considering factors such as throughput, cycle time, and potential bottlenecks.
- Optimize the design iteratively based on simulation results.

# For more details and insights, you can access my portfolio. 🚀
https://sites.google.com/kletech.ac.in/daiviksportfolio/home
