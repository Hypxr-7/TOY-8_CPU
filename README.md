
# TOY-8 CPU in Logism

The following is a TOY-8 CPU, a simplified version of the TOY CPU.

# PREREQUISITES

The above circuit is build using Logism-Evolution.\
https://github.com/logisim-evolution/logisim-evolution

# How To Use

• Open the circuit in Logism-Evolution.\
• Go to the Interface circuit to view the user controls.\
• To begin inputting your program, first enable Auto-Tick from the Simulate Tab.\
• Ideally set the Auto-Tick Frequency to 2Hz, but faster work as well.\
• Then load your program by inputting the address and the data.\
• Once done, disable Auto-Tick and if the clock is high, click it one to set it to low.\
• Also set the data and address input to 0.\
• Then click on the RUN button to enable the CPU. This will be evident by the LED turning green.\
• Then just enable Auto-Tick again and watch it run.\
• It will come to halt at the end of the program.

# INSTRUCTION SET 

| Opcode | Operation | Pseudocode |
|--------|-----------|------------|
|   0    | Halt     | Halt  |
|   2    | Add      |  R = R + M[addr] |
|   4    | Bitwise AND |  R = R & M[addr] |
|   6    |   Bitwise XOR| R = R ^ M[addr]  |
|   8    |   Load Addr |  R = addr |
|   A    |   Load|  R = M[addr] |
|   C    |   Store|  M[addr] = R |
|   E    |   Branch|  if (R == 0) PC = addr |






