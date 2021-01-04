AArch64 Cross Compiler
======================

Before we could start our tutorials, you'll need some tools. Namely a compiler that compiles for the AArch64
architecture and it's companion utilities.

**IMPORTANT NOTE**: this description is not about how to compile a cross-compiler in general. It's about how to
compile one specifically for the *aarch64-elf* target. If you have problems, google "how to build a gcc cross-compiler"
or ask on an appropriate support forum for your operating system. I can't and won't help you with your environment,
you have to solve that on your own. As I've said in the introduction I assume you know how to compile programs
(including the compilation of the cross-compiler).

Each directory has two Makefiles, one for the GNU gcc, and one for LLVM clang. Pick the one you prefer. I could have used makefile
variables and a common configuration, but it was important that each tutorial must be self-contained and dependency-free.

**install in Ubuntu:**
```
sudo apt-get install gcc-aarch64-linux-gnu
```

**check it:**
```
aarch64-linux-gnu-gcc -v
```
