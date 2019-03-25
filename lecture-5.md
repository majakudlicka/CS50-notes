Physical memory addresses - often prefixed with 0x: hexadecimal (16 digits: 1-9 + a-f)
Convenient because each digit represents 4 bits

t[i] = s[i] <=> *(t+1) = *(s+i)

Computer's RAM

- Text
-Initialised data
-Uninitialised data
- Heap
-Stack
-Env variables

Stack overflow - a situation in which programs has exceeded its allocated memory and starts overwriting values in places it shouldn't.
Often malicious. If hacker manages to override return memory address, they can insert and execute malicious code.

What goes on in compiler:

1. Pre-processing
2. Compiling
3. Assembling
4. Linking

Lines at the begining of the program prefixed with hash - preprocessor directives = lines of code that get converted into something else before program tries to convert it to machine language (pre-processing)

Linking= combining your compiled code with other libraries' compiled code

Head = part of memory that is longer-lived than stack. We use it when we want functions to keep some values in memory after the end of their execution. Memory can run out if our program requests too much of it (infinite loops but not only)

Valgrind: program that checks for memory leaks in C

malloc != free

Array index notation starts at 0 (like JS)

Convention in C- returning special value in case of error, e.g. CHAR_MAX

typedef: used to declare a custom data structure 

. -> accesses props on objects
