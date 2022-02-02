# Description of the all instructions for Gofra bytecode.
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
|`SH`       ||
|`CP`       ||
|`CP2`      ||
|`CPO`      ||
|`FR`       ||
||**I/O operations**|
|`IORS`     ||
|`IORI`     |Requires user to enter input, and pushes -1 (if invalid input) or integer of the input|
||**Memory operations**|
|`MPTR`     ||
|`NULL`     ||
|`MW`       |Pops two elements from the stack, where head is value to write and second is pointer to write, and writes 1 byte to the memory|
|`MR`       ||
|`MW4`      ||
|`MR4`      ||
|`MSC`      ||
