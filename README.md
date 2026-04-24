*This project has been created as part of the 42 curriculum by gdosch.*

# Push_swap

## Description
The **Push_swap** project is a highly structured algorithmic challenge from the 42 curriculum. The objective is simple yet complex: you must sort a random list of integers using two stacks (`a` and `b`) and a strictly limited set of instructions, aiming for the lowest possible number of operations.

This project introduces concepts of algorithmic complexity and optimization. Sorting algorithms must be chosen and tailored to efficiently handle varied input sizes, such as passing a benchmark of 100 randomly placed integers in under 700 operations, and 500 integers in fewer than 5500 operations.

### The Rules
- **Stack A:** Starts with a random number of unique integers.
- **Stack B:** Starts empty.
- **Goal:** Sort `stack a` in ascending order (smallest number at the top).
- **Allowed Operations:**
  - `sa`, `sb`, `ss`: Swap the first 2 elements at the top of the stack(s).
  - `pa`, `pb`: Push the first element from one stack to the other.
  - `ra`, `rb`, `rr`: Rotate the stack(s) upwards (first element becomes last).
  - `rra`, `rrb`, `rrr`: Reverse rotate the stack(s) downwards (last element becomes first).

## Instructions

### Compilation
The project includes a `Makefile` to compile the source code. The following standard rules are available:
- `make` or `make all`: Compiles the `push_swap` binary.
- `make clean`: Removes object files.
- `make fclean`: Removes object files and the executables.
- `make re`: Recompiles the whole project.
- `make bonus`: Compiles the bonus `checker` binary.

### Execution

#### push_swap (Mandatory)
Run the program by providing a list of integers as arguments. The program will output the sequence of instructions needed to sort the stack.
```bash
./push_swap 2 1 3 6 5 8
```

#### checker (Bonus)
The checker program reads a list of instructions from standard input and applies them to the provided list of integers. It outputs `OK` if the stack is sorted, and `KO` otherwise.
```bash
./push_swap 2 1 3 6 5 8 | ./checker 2 1 3 6 5 8
```

## Resources
- **Algorithms:** Conceptually, solutions often implement variations of established algorithms such as Radix Sort, Quick Sort, or custom insertion sorts (like the "Turk Algorithm").
- **Complexity Analysis:** Understanding Big-O notation is essential to minimize the number of operations. 
- **AI Usage:** Generative AI tools were consulted to better understand the time complexity characteristics of various sorting algorithms, help conceptualize edge cases for error testing, and assist in drafting the required structure of this README file. No AI generated code was used without full understanding and adaptation to the project's strict normative constraints.
