## Ghidra Sega Saturn Loader

A (WIP) loader and processor for Ghidra for Sega Saturn files. Currently:
- able to disassemble SH2 after manually specifying processor type. I used the instruction encodings available from [Renesas SH Instruction Set Summary](http://shared-ptr.com/sh_insns.html) and related github project [shared-ptr/sh_insns](https://github.com/shared-ptr/sh_insns). 
- contains SLEIGH definitions for ~99% of instructions. Debugging issues related to sign extensions, flags, and branches. 
- able decompile automatically. Output is wonky due to issues in the SLEIGH definitions.

Todo: 
- fix errors in SLEIGH definitions
- Sega Saturn memory map
- automatic detection and loading of Sega Saturn files

## Screenshots

Loader screenshot  
![Loader](screenshot_loader.png)

Disassembly View (Decompiler somewhat working, lots of bugs)  
![Disassembly View](screenshot_loaded.png)

## Issues
I anticipate lots of bugs. It will take time to correct errors in the SLEIGH definition. 

## Installation
- Rename the root folder to SH2 and copy it to Ghidra/Processors/ and restart Ghidra

## Credits
- [shared-ptr/sh_insns](https://github.com/shared-ptr/sh_insns)
- [xyzz/ghidra-mep](https://github.com/xyzz/ghidra-mep)




