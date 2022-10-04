# C - Search Algorithms

This was my Holberton School project on search algorithms. I implemented
various types of search algorithms and stated the corresponding space/time
complexities for each.

## Tests :heavy_check_mark:

* [tests](./tests): Folder of test files for all tasks. Provided by Holberton
School.

## Helper Files :raised_hands:

* [listint](./listint): Folder of helper files for task 12, singly linked list
jump search.
  * [create_list.c](./listint/create_list.c): C function that creates a `listint_t`
singly linked list.
  * [free_list.c](./listint/free_list.c): C function that frees a `listint_t`
singly linked list.
  * [print_list.c](./listint/print_list.c): C function that prints the contents
of a `listint_t` singly linked list.

* [skiplist](./skiplist): Folder of helper files for task 13, singly skipped list
jump search.
  * [create_skiplist.c](./skiplist/create_skiplist.c): C function that creates
a `skiplist_t` singly skipped list.
  * [free_skiplist.c](./skiplist/free_skiplist.c): C function that frees a
`skiplist_t` singly skipped list.
  * [print_skiplist.c](./skiplist/print_skiplist.c): C function that prints the
contents of a `skiplist_t` singly skipped list.

## Header File :file_folder:

* [search_algos.h](./search_algos.h): Header file containing definitions and
prototypes for all types and functions written for the project.

Data Structures
```
/**
 * struct listint_s - singly linked list
 *
 * @n: Integer
 * @index: Index of the node in the list
 * @next: Pointer to the next node
 *
 * Description: singly linked list node structure
 * for Holberton project
 */
typedef struct listint_s
{
    int n;
    size_t index;
    struct listint_s *next;
} listint_t;

/**
 * struct skiplist_s - Singly linked list with an express lane
 *
 * @n: Integer
 * @index: Index of the node in the list
 * @next: Pointer to the next node
 * @express: Pointer to the next node in the express lane
 *
 * Description: singly linked list node structure with an express lane
 * for Holberton project
 */
typedef struct skiplist_s
{
    int n;
    size_t index;
    struct skiplist_s *next;
    struct skiplist_s *express;
} skiplist_t;
```

