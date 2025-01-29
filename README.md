# Running C Program on Linux

## Prerequisites

Ensure that you have the GCC compiler installed on your system. You can check by running:

```sh
gcc --version
```

If GCC is not installed, you can install it using:

```sh
sudo apt update && sudo apt install gcc  # For Debian/Ubuntu
sudo yum install gcc  # For RHEL/CentOS
sudo dnf install gcc  # For Fedora
```

## Writing a C Program

Create a new C file using a text editor:

```sh
nano hello.c
```

Add the following simple C program:

```c
#include <stdio.h>

int main() {
    printf("Hello, Linux!\n");
    return 0;
}
```

Save the file and exit the editor.

## Compiling the C Program

Compile the program using GCC:

```sh
gcc hello.c -o hello
```

This creates an executable file named `hello`.

## Running the Compiled Program

Run the compiled program with:

```sh
./hello
```

Expected output:

```
Hello, Linux!
```

## Debugging and Compilation Options

To enable debugging, use:

```sh
gcc -g hello.c -o hello
```

To enable warnings and optimizations:

```sh
gcc -Wall -O2 hello.c -o hello
```

