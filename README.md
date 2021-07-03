# Shell in C

This project is a simple implementation of an unix shell (LSH) in C.  It demonstrates the basic functionalities of a shell.
That is: read, parse, fork, exec, and wait. Since my purpose was to learn how shell works and build basic functionalities, this shell is not meant for feature completeness 
or even fitness for casual use. 

It has many limitations, including:

* Commands must be on a single line.
* Arguments must be separated by whitespace.
* No quoting arguments or escaping whitespace.
* No piping or redirection.
* Only builtins are: `cd`, `help`, `exit`.

## Installation and Setup Instructions

### Prerequisites (Requirements):

C program can be written and executed on any machine that has a suitable environment to run the program.
It is recommended using an IDE to run C programs. An IDE includes a compiler, editor and debugger. Clanfg, MinGW compiler (Minimalist GNU for Windows), Portable 'C' compiler, and Turbo C are popular compilers available. I am using [GCC Compiler](https://gcc.gnu.org).

Here is the [link](https://www.guru99.com/c-gcc-install.html) to download GCC Complier for Windows, Linux and Mac.

### How to Use/Run:

**Compile:**

`gcc -o lsh src/main.c` 

**Run:** 

`./lsh` 

If you would like to use the standard-library based implementation of `lsh_read_line()`, then
you can do: 

`gcc -DLSH_USE_STD_GETLINE -o lsh src/main.c`.

License
-------

MIT License
Copyright (c) 2021 Daljeet Singh

Refer to **LICENSE** file for full information.
