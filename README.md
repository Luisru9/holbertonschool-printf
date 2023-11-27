echo -e "\033[1;37mPrintf Group Projects\033[0m"


Description 💬

 formatted output conversion #include "main.h" int _printf(const char format , ...);

The _printf() function produce output according to a format as described below. Also, write output to stdout, the standard output stream. The _printf() function write the output under the control of a format string that specifies how subsequent arguments (or arguments accessed via the variable-length argument facilities of stdarg(3) are converted for output.

Format of the format string The format string is a character string, beginning and ending inits initial shift state, if any. The format string is composed of zero or more directives: ordinary characters (not %), which are copied unchanged to the output stream; and conversion specifications, each of which results in fetching zero or more subsequent arguments. Each conversion specification is introduced by the character % and ends with conversion specifier.

Conversion specifiers A character that specifies the type of conversion to be applied. The conversion specifiers and their meaning are:

d, i: The int argument should be signed decimal notation, and the resulting number is written.
c: The int argument is converted to a char, and the resulting character is written.
s: The const char * argument is expected to be a pointer to an array of character type (pointer to a string). Characters from the array are written up to (but not including) a terminating null byte ('\0').
%: A '%' is written. No argument is converted. The complete conversion specification is '%%'.

Task 📃


~~~ c int _printf(const char *format, ...) - is used for formatted output. It's akin to the standard printf function and allows developers to print formatted text to the standard output.

int print_c(va_list args)| - a function used within a custom printf-like function to handle the printing of a single character specifier, often denoted by %c in the format string.

int _printf(const char *format, ...) - is used for formatted output. It's akin to the standard printf function and allows developers to print formatted text to the standard output.

int print_c(va_list args)- a function used within a custom printf-like function to handle the printing of a single character specifier, often denoted by %c in the format string.

int print_s(va_list args) - function to handle the printing of strings, often denoted by the %s specifier in the format string.

int print_percent(va_list args) -  function to handle the printing of the literal % character, typically denoted by %% in the format string.

int print_d(va_list args) - function specifically designed to handle printing decimal integers, often associated with the %d specifier in the format string.

int print_i(va_list args) - function to handle the printing of integer values, similar to the %i specifier in the format string.

int (*get_func(char x))(va_list)  - function get_func that takes a character x as an argument and returns a pointer to a function that takes a va_list as an argument and returns an integer.

int (*get_func(char x))(va_list) - function get_func that takes a character x as an argument and returns a pointer to a function that takes a va_list as an argument and returns an integer.

Return Value Upon successful return, the _printf() function return the number of characters printed (excluding the null byte used to end output to strings). If an output error is encountered, a negative value is returned.

Authors ✒️

 _printf() is written and maintained by Luis Gonzales and Aaron M. Lopez.

