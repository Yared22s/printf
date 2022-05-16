Printf Group Project Readme.

printf is a weel known function used in C programming to do formated printing. 
Usually it only takes the standard library  <stdio.h> to call it into a c program, 
and using it for simple strings or formatted specifiers that allow us to print diferent types of data. 

This project ask us to develop a printf function made from scratch in most of its features in order to understand the complexity of a powerful tool. 
For further study refer man 3 of printf to understand how _printf works.

For Compilation purpose We use 

```$ gcc -Wall -Werror -Wextra -pedantic *.c``` /*"*=> refers the function name"*/


For testing Prototype

```int _printf(const char *format, ...)```

If everything is succesful the function returns the number of characteres printed using the below format.

| Specifiers      | Description |
| ----------- | ----------- |
| %c  | Print single character |
| %s  | Print string of characteres |
| %d  | Print decimal numbers|
| %i  | Print integers |

The Project files and there description

 File        | Description |
 
| main.h is the **Header file** 
				Include all  function prototypes, Include structure of specifiers.
				
| printf.c is the **Project function: _printf** 
				Start the variadic list. Iterates string  format of entry and check for a moldule symbol (%).
				If the symbol is found then check if the next char match with one of the valid specifiers in the structure using
				the auxiliar function to comapare (comp),in that case the respective function of these format is called for the 
				characters that doesn't match any of the formats the function ignores the module symbole and print it  as a string.
				In case that the module symbole is not found, print the each character normally.
				
| printf_functions.c is the **Auxiliar functions**_putchar: using write function, 
	prints a character printc: 
	print character using list variable.
    print_string: pint strings, if string is null it pirnts (null) print_n: print numbers base 10.

 Contributors

	Yared Sitotaw
	Zerubabel Tore


	
