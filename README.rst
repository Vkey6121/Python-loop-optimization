************
Python loop optimization for numerical calculations
************

This is the companion code for article `"If you have slow loops in Python, you can fix it…until you can’t" <https://medium.freecodecamp.org/if-you-have-slow-loops-in-python-you-can-fix-it-until-you-cant-3a39e03b6f35>`_

- ks_dp_solvers.py - a number of solver functions implementing dynamic programming algorithm to solve the knapsack problem. Solvers employ different approaches to looping through the array of data. 
- ks_dp_solvers_profiles.txt - outputs of line profiler for the above implementations
- ks_dp_cython.pyx - a straightforward solver (two nested for loops) based on cython
- ks_dp_cython_script.py - the script to run ks_dp_cython.pyx
- ks_dp_naive_solver.go - a straightforward solver (two nested for loops) coded in Golang
- nasdaq100list.csv - data file (Nasdaq 100 list of stock prices and price estimates)
- ks_dp_example.pdf - an annotated illustration of the dynamic programming algorithm used to solve the knapsack problem

Project Highlights:

Loop Unrolling: Implement loop unrolling to reduce loop overhead and increase instruction-level parallelism, resulting in improved execution speed.
Vectorization: Utilize SIMD (Single Instruction, Multiple Data) instructions and vectorized operations to process multiple data elements simultaneously, enhancing parallelism and optimizing mathematical operations.
Memory Locality Enhancement: Apply memory access optimization techniques to enhance cache locality, minimizing data transfer overhead and improving memory access patterns.
Benchmarking Suite: Develop a suite of benchmark tests to evaluate the performance of the optimized loops against the original implementations, providing quantifiable performance metrics.
Profiling and Analysis: Employ profiling tools to identify performance bottlenecks and optimize critical sections of the code based on runtime characteristics.
Documentation and Visualization: Create comprehensive documentation outlining the optimization techniques used, performance improvements achieved, and code examples. Visualize benchmark results for easy comparison.
