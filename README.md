# Julia-Set-Calculation-using-MPI


## Description

This program calculates the **Julia Set**, a fractal formed by iterating over a complex function. Using MPI, the program distributes the computation of the Julia set for a grid of complex numbers.

## Requirements

- **Language**: C/C++ (recommended), Python
- **Framework**: MPI

## Input Format

- The first line contains three integers `N`, `M`, and `K` representing the grid size and the number of iterations.
- The second line contains two floating-point numbers representing the real and imaginary parts of the constant `c`.

## Output Format

- Print the `N × M` grid of ones and zeros, where 1 indicates the point belongs to the Julia set and 0 indicates it does not.

## Example

### Input
```
25 25 10
-0.75 0.25
```

### Output
```
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
...
```

## How to Run

1. Compile the program:
   ```bash
   mpicc -o julia 2.cpp
   ```

2. Run the program with MPI:
   ```bash
   mpiexec -np <number_of_processes> ./julia <input_file>
   ```

---
