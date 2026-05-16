# ft_printf

A custom implementation of the standard C `printf()` function developed as part of the 42 curriculum.

## About

The goal of ft_printf is to recreate the behavior of the original `printf()` function from the C standard library.

This project focuses on:
- Variadic functions
- String formatting
- Memory management
- Base conversions
- Low-level output handling
- Modular programming in C

ft_printf became an important step in understanding how formatted output works internally.

---

## Features

Supported conversions:

| Specifier | Description |
|----------|-------------|
| `%c` | Character |
| `%s` | String |
| `%p` | Pointer address |
| `%d` | Signed decimal integer |
| `%i` | Integer |
| `%u` | Unsigned decimal integer |
| `%x` | Lowercase hexadecimal |
| `%X` | Uppercase hexadecimal |
| `%%` | Percent sign |

---

## Compilation

Available rules:
```bash
make
make bonus
make clean
make fclean
make re
```

## Example

```bash
#include "ft_printf.h"

int main(void)
{
    ft_printf("Hello %s!\n", "42");
    ft_printf("Number: %d\n", 42);
    ft_printf("Hex: %x\n", 255);

    return (0);
}
```

Output:

```bash
Hello 42!
Number: 42
Hex: ff
```

## Implementation Details

This project was built using:

- Variadic arguments with stdarg.h
- Custom number conversion functions
- Low-level write() system calls

The project does not use the original printf() internally.

## Compliance

This project was developed in compliance with the requirements and constraints of the 42 network, respecting the imposed coding standards, allowed functions, and project guidelines.
