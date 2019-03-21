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


