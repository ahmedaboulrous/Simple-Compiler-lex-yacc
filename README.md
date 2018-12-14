# Simple-Compiler-lex-yacc
An implementation of a simple-compiler ( scanner and parser ) using lex and yacc.

- description
    - scanner.l : contains tokens to be identified.
    - parser.y  : contains grammar rules for the language.
                  generates "y.tab.h" header containing tokens for the scanner to identify.
                  generates "y.tab.c" which is compiled along with "lex.yy.c" to generate
                  the interpreter "mylang" 

- compilation (lex and yacc)
    - yacc parser.y
    - lex scanner.l
    - gcc y.tab.c lex.yy.c -o mylang.out
    - ./mylang.out

- Running
    - running the mylang executable will give you an interactive interpreter.
    - you can use print to the standard output using "print expr;" command;
    - you can exit out of the interpreter using the "exit;" command. 

- Language
    - variables:  are one letter long [a-z and A-Z], stores floating-point numbers
    - operations: you can perform +, -, *, / on the variables


