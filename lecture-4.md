Insertion sort cont'd
Omega: n

Constant number of steps - being simplified to O(n) - for example accessing the variable

MergeSort:
O: n logn
Omega: n longn

logn - comes from the dividing by 2 part
n - comes from the merging part

If O happens to be the same as Omega, we can descirbe it as Theta

MergeSoer pseudocode:

If n < 2
  return
Else:
  Sort left half of elements.
  Sort right half of elements.
  Merge sorted halves.
  
Mergesort takes up more memoru than more 'primitive' sorting algorithms

T(n) = T(n/2) + T(n/2) + n, if n >1 (+n -> merging)

T(16) = 2 x T(8) + 16
T(8) = 2 x T(4) + 8
T(4) = 2 x T(2) + 4
T(2) = 2 x T(1) + 2
T(1) = 0

T(16)= 64 = 16log16 = n logn!!

The way C represents negative numbers is by changing one bit. For very large positive numbers, it might get confused...

Adding * to variable name (ex int* a) indicates that we intend to pass it as a link to an address in memory, not as a copy 

We use & when calling a function and * when declaring it

* --> "Go to location..."

string in C - an address of the character in RAM

Char - typically 1 byte. Int - typically 4 bytes.

String in C is an array of chars, being 1 byte apart from each other and terminated by special \o character indicating the end of string.

string = char*

'getString()' actualy returns the address of the first byte. That is sufficient to find the entire string.

This is why comparing strings using == in C actually compares addresses in memory under the hood and returns false for identical strings.

0th byte: reserved for signalling errors. No data is ever stored there. 0 == NULL

When you 'naively' copy string in C, they are being copied by reference - point to the same address in memory.

String.h -> you can find string compare function there

Malloc: memmory allocation

In C, when you are dealing with address, it usually means the first address of the requested chunk.

When you put a string in memory, you should ask for its length + 1 bytes -> 1 reserved for special /o character.

Sizeof - function that will tell you how many bytes a given data type requires. For example, sizeoOf(char) = 1 (typically)

If for whatever reason memmory could not be allocated, system will return NULL.



