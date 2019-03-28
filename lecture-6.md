buffer, string - it already is memory so we can pass it straightaway, we don't need a pointer

Sometimes you don't need malloc, you can achieve the same by doing, for instance, char buffer[16]

struct - new data structure

When you delete the file from trash, computer 'forgets' what was at the memory location and it is available to be overwritten.
But it doesn't get overwritten unless you save new files, immediately after remove action info is still there.

There are certain patterns that camn be associated, for example, with the beginning of the jped image.

Arrays - fixed size, all boxes in memory are next to each other - we only need to know the first address -> arrays give us random access.
Just by using [i] we can access any element in constant time

Linked list - a list of nodes - values and pointers

typedef struct node
{
  int n;
  struct node* next;
}
node;

Operations we can perform on link list: insert, delete, search, traverse

To access a struct from pointer ptnr->n (arrow)(like . but when we have a pointer)

Linked lists need more memory space than arrays

Last elememt's pointer = NULL

Convention - put datatype definitions at the top of the file


