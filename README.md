# Description of the all instructions for Gofra bytecode.
### Bytecode implements simple stack-machine with push/pop operations.
### Strings (Not currently implemented in virtual machine / bytecode) will be represented as size+pointer to the memory.

|Operation|Description|
|---------|-----------|
||**Binary math operations**|
|`+`        |Pops two elements from the stack, and push their sum back|
|`-`        |Pops two elements from the stack, and push their difference back|
|`*`        |Pops two elements from the stack, and push value of them multiplicated where head of the stack - multiplier|
|`/`        |Pops two elements from the stack, and push value of them divided where head of the stack - dividor|
|`==`       |Pops two elements from the stack, and push 0 or 1|
|`!=`       |Pops two elements from the stack, and push 0 or 1|
|`<`        |Pops two elements from the stack, and push 0 or 1|
|`>`        |Pops two elements from the stack, and push 0 or 1|
|`>=`       |Pops two elements from the stack, and push 0 or 1|
|`--`       |Same as `1 -`|
|`++`       |Same as `1 +`|
||**Stack manipulation operations**|
|`SW`       ||
|`SH`       |Pops one element from the stack and show it on the screen|
|`CP`       |Pops one element from the stack and push 2 new (Copy element)|
|`CP2`      ||
|`CPO`      ||
|`FR`       |Pops one element from the stack and removes it (Free)|
||**I/O operations**|
|`IORS`     |Requires user to enter input, and pushes string. (Size + pointer)|
|`IORI`     |Requires user to enter input, and pushes -1 (if invalid input) or integer of the input|
||**Memory operations**|
|`MPTR`     ||
|`NULL`     |Push NULL (0) to the stack|
|`MW`       |Pops two elements from the stack, where head is value to write and second is pointer to write, then writes value as 1 byte to the memory|
|`MR`       ||
|`MW4`      |Same as `MW`, but writes values 4 bytes|
|`MR4`      |Same as `MR`, but reads value as 4 bytes|
|`MSC`      ||
