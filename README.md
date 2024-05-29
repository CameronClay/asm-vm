# Assembler and Virtual machine
Two-pass assembler which converts assembly code into byte-code which can then be run on the virtual machine. Based on Reduced Instruction Set Computing (RISC) architecture.

## How to run
```
Arugments: vm [-dump] [-log] [-mem_sz #KB] [-max_thrd #] [-inst_per_thrd #]

[-dump]            Outputs the bytecode (.byt) to a file rather than running it.
[-log]             Enables debugging.
[-mem_sz #]        Allocates #KB for use for assembling and running in the virtual machine.
[-max_thrd #]      Specifies the maximum number of threads the virtual machine will support. Making use of the threads requires use of multithreaded instructions.
[-inst_per_thrd #] Specifies how many instructions are run per thread before initiating a context switch.
```

### Unit Testing
- Unit testing done with Boost.Test.

### Tooling
- C++ 20 (with **C++ 20 modules**)
- CMake
- Boost.Test
- vcpkg
- Visual Studio Code

### Note
The code for this project is private but I am more than happy to show and explain the code.
