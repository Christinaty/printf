# 0x11. C - printf 

- Writing our own `printf` function, this is a project done under **ALX Low Level Programming**

## Resource

- [secrets of printf](https://www.cypress.com/file/54761/download)
- [Implementing printf and scanf in C](https://iq.opengenus.org/how-printf-and-scanf-function-works-in-c-internally/)
- [All About Printf](https://akshatshibu.wordpress.com/2015/07/22/all-about-printf/)


## Description

- The function `_printf` writes output to stdout. The function writes under the control of a `format` string that specifies how subsequent arguments (accessed via the variable-length argument facilities of standard library `stdarg`) are converted for output.

- Prototype: `int _printf(const char *format, ...);`

## Return

- Upon success, `_printf` returns the number of characters printed (**excluding the terminating null byte used to end output to strings**). If an output error is encountered, the function returns `-1`.

## Format of the Argument String

- The `format` string argument is a constant character string composed of zero or more directives: ordinary characters (apart from `%`) which are copied unchanged to the output stream; and conversion specifications, each of which results in fetching zero or more subsequent arguments.
- Conversion specification is introduced by the character `%` and ends with a conversion specifier (which in whole make up the format specifier.)

## General Requirements

- All your files will be compiled on Ubuntu 20.04 LTS using `gcc`, using the options `-Wall -Werror -Wextra -pedantic -std=gnu89`
- All your files should end with a new line.
- No more than 5 functions per file.
- You are not allowed to use global variables.
- The prototypes of all your functions should be included in your header file called `holberton.h`
- All your header files should be include guarded.

### Authorized functions and macros

- `write` (`man 2 write`)
- `malloc` (`man 3 malloc`)
- `free` (`man 3 free`)
- `va_start` (`man 3 va_start`)
- `va_end` (`man 3 va_end`)
- `va_copy` (`man 3 va_copy`)
- `va_arg` (`man 3 va_arg`)

### Github

- There should be one project repository per group. If you clone/fork/whatever a project repository with the same name before the second deadline, you risk a 0% score.

### Compilation

- The code can be compiled like this:
	```sh
	gcc -Wall -Werror -Wextra -pedantic -std=gnu89 test/main.c *.c -o print
	```
- All test files will be in the [test](./test) directory.
---
### Format Specifiers

The _printf program will replicate the effects of the listed % format specifiers as when used with printf.

Function name | Description | Format Specifier
--- | --- | ---
`_print_char` | Prints a single character | `%c`
`_print_string` | Prints a string of characters | `%s`
`_print_percent` | Prints a % | `%%`
`_print_int` | Prints an integer in base 10| `%d` & `%i`
`_print_reverse` | Prints the string in reverse | `r`
`_print_rot13` | Converts the string into Rot13 | `R`
`_print_binary` | Prints the binary form of the integer | `b`
`_print_unsigned` | Prints an unsigned integer | `u`
`_print_octal` | Prints and octal number | `o`
`_print_hex_l` | Prints the lower case hexidecimal number | `x`
`_print_hex_u` | Prints the upper case hexidecimal number | `X`
---
<div align="center">

### AUTHORS

- Adegbaju, Christina [https://github.com/Christinaty](./https://github.com/Christinaty)
- Jonathan, Boomni Oye [https://github.com/Boomni](./https://github.com/boomni)
</div>
