# C++ Off-by-One Error Example
This repository demonstrates a common off-by-one error in C++ when iterating over a `std::vector`.  The error occurs when the loop condition `i <= vec.size()` allows access to an element beyond the valid range of the vector.

## Bug Description
The bug is a simple off-by-one error. The loop attempts to access one element past the end of the vector, leading to undefined behavior. This could manifest as a program crash, incorrect output, or seemingly random results. 

## Solution
The solution involves changing the loop condition to `i < vec.size()`, ensuring that the loop iterates only up to the last valid index of the vector.  This prevents accessing elements beyond the vector's bounds.