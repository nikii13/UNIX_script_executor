# UNIX Script Executor

An operating systems coursework project implementing a simple script interpreter in C using POSIX system calls.

## Features
- Command tokenization and execution with `fork` and `execvp`.
- Pipeline handling using `pipe` and `dup2`.
- Standard input, output and error redirection.
- Foreground and background process handling.
- A companion `mygrep` utility and example scripts.

## Build and run
On Linux or WSL, with GCC and Make:

```sh
make
./scripter script.txt
make clean
```

Script files must start with the header `## Script de SSOO`. Only execute trusted scripts: this program launches local commands.

This is an educational implementation, not a production shell. See the [original collaborative repository](https://github.com/aryanv175/p2_scripter) for project history and attribution.
