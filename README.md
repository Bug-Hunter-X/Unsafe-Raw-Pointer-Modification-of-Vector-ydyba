# Unsafe Raw Pointer Modification of Vector in Rust

This repository demonstrates a potential error when using raw pointers to modify a Rust vector. Directly modifying the vector's memory using a raw pointer can cause issues if the vector's internal layout changes.  The solution showcases safer alternatives.

## Bug
The `bug.rs` file shows how modifying a vector using `as_mut_ptr()` and unsafe code can result in undefined behavior.

## Solution
The `bugSolution.rs` file provides a safe and correct method to modify the vector's contents using indexing or iterators, avoiding the risks of using raw pointers.