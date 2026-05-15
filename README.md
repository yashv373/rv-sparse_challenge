# RV-Sparse Coding Challenge

Simple implementation of `sparse_multiply` for the [rv-sparse](https://github.com/merledu/rv-sparse) LFX Mentorship coding challenge.

## What it does

The function takes a dense matrix `A` and a vector `x`, and computes `y = A * x`. But instead of doing it the normal way (which wastes time multiplying zeros), it:

1. First converts the matrix into CSR format (only stores non-zero values)
2. Then does the multiplication using only those non-zero values

No `malloc` or `free` is used inside the function — all memory is provided by the caller.

## How to build and run

```bash
gcc -o run code.c -lm
./run
```

You should see: `All tests passed! (100/100 iterations passed)`

## Author

Yashvardhan Singh
