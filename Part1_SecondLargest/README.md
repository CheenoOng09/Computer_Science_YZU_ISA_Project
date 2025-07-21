# Part 1 – YZU-ISA Assembly Program: Second Largest Number

## Problem Description

Given `n` integers (including duplicates), find the **second largest number**.  
If no distinct second-largest exists (e.g., all values are equal), return the **largest number**.

- Input:  
  - First line: number of test cases  
  - For each test case:
    - First line: number of integers `n`
    - Next `n` lines: one integer per line

- Output:
  - For each test case, print the second largest number.

## 🔧 Implementation

- Language: **YZU-ISA Assembly**
- Operations:
  - Read test cases and inputs using `LOAD`, `STOREI`
  - Sort array using nested loops and conditional jumps
  - Identify second largest number via reverse traversal

## Files Included

- `Revised_Proposal_with_Screenshot.pdf`: Problem spec and expected behavior
- `Code_1103558.txt`: Fully commented YZU-ISA assembly code
- `In_1103558.txt`: Input used for testing
- `Out_1103558.pdf`: Screenshots proving correctness of results

## Sample Output

Example 1 Input:
```
2 <--- Number of Test Case
4 <--- Number of Integers in the first test case
9
9
7
7
4 <--- Number of Integers in the second test case
-1
6
8
5
```
Example 1 Output:
```
7 <--- Output from the first test case
6 <--- Output from the second test case
```


## 🛠 Features

- Full bubble sort using address-based storage
- Handles repeated values and outputs correctly even when only one unique number
- Modular and clear code structure with comments
