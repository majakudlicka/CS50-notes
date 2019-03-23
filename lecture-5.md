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
