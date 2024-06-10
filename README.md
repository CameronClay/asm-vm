# Assembler and Virtual machine
Two-pass assembler which converts assembly code into byte-code which can then be run on the virtual machine. Based on Reduced Instruction Set Computing (RISC) architecture.

## How to run
```
Allowed options:
  -h [ --help ]                   Produce help message
  -m [ --mem-sz ] arg (=2)        Specifies the amount of memory in MB for use
                                  in assembling and running in the virtual
                                  machine.
  -t [ --max-thrd ] arg (=15)     Specifies the maximum number of threads the
                                  virtual machine will support. Making use of
                                  the threads requires use of multithreaded
                                  instructions.
  -f [ --input-file ] arg         Specifies the source file to be assembled and
                                  run.
  -l [ --log ] arg (=log.dat)     Enables debug logging to specified filename
                                  via TRAP calls.
  -i [ --inst-per-thrd ] arg (=1) Specifies how many instructions are run per
                                  thread before initiating a context switch.
  -d [ --dump ]                   Output the bytecode to a .byt file instead of
                                  running it (incompatible when loading a .byt
                                  file).
```

### Unit Testing
- Unit testing done with Boost.Test.

### Tooling
- C++ 20 (with **C++ 20 modules**)
- CMake
- Boost.Test
- Boost.Program_options
- vcpkg
- Visual Studio Code
- MSVC compiler

### Note
The code for this project is private but I am more than happy to show and explain the code.
