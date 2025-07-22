# Part 3 – Implementation of Proposed Problem: Average of Odd and Even Numbers

## Problem Description

This YZU-ISA assembly program solves the problem of calculating the **average** of odd and even numbers separately from a given list of integers.

For each test case:
- Read `n` integers.
- Separate them into **odd** and **even** groups.
- Compute the **average** and **remainder** for both groups.
- If a group has no integers, return a default value (`1` for odd, `2` for even).
- If only one test case is run, the program will still print the correct output format.

Example:
Input: → 5, 50, 17, 88, 2, 63, 7, 5, 11, 90
Odd Avg: → 18 (remainder: 0)
Even Avg: → 57 (remainder: 2)


## Files

| File Name              | Description                                 |
|------------------------|---------------------------------------------|
| `Code_1103558.txt`     | YZU-ISA assembly source code                |
| `In_1103558.txt`       | Sample input file for test cases            |
| `PR_1103558.pdf`       | Problem statement and description           |
| `Out_1103558.pdf`      | Screenshot of the output                    |

## Implementation Notes

- **Registers Used**:
  - `R4`: Pointer to original array
  - `R6`: Pointer to odd group array
  - `R7`: Pointer to even group array
  - `R10`: Counter for odd numbers
  - `R11`: Counter for even numbers
  - `R8`: Used for sum accumulation
  - `R3`: Used for storing average result
- Uses loops to:
  - Input array
  - Check parity
  - Separate odd and even
  - Accumulate sums
  - Compute integer division using subtraction
- Handles zero, single, and multiple values robustly.

## Input Format

- First line: number of test cases
- For each test case:
  - First line: number `n`
  - Next `n` lines: one integer per line

Example:
```
1 <--- Number of test case
10 <--- Number of Integers
24
13
19
4
7
8
33
7
20
4
...
```

## 📤 Output Format

For each test case:
`<Odd Average>` `<Odd Remainder>` `<Even Average>` `<Even Remainder>`

Example:
```
15 <--- Odd Average Result
4  <--- Odd Remainder
12 <--- Even Average
0  <--- Even Remainder
...

```
