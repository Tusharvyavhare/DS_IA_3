# Data Structures Internal Activity 3

## Project Title
Personalized Hash Table Implementation Using Division Method and Linear Probing

## Student Details
- **PRN:** 202602100010
- **Subject:** Data Structures
- **Programming Language:** C++

## Project Description
This project implements a hash table using the Division Method and Linear Probing for collision handling.

The project uses a personalized dataset generated according to the student's PRN. It demonstrates how hashing maps keys to table indices and how linear probing resolves collisions.

## Personalized Dataset

PRN last four digits (S) = 10

The dataset is generated using:

`v[i] = (S + 13 * i) mod 100`

Dataset:

`10, 23, 36, 49, 62, 75, 88, 1, 14, 27, 40, 53, 66, 79, 92, 5, 18, 31, 44, 57`

## Hashing Details
- Hashing technique: Division Method
- Collision handling: Linear Probing
- Table size: 10 (implementation assumption; confirm with faculty)
- Programming language: C++

Hash function:

`h(key) = key mod 10`

## Project Files
- `README.md`: Project overview and documentation.
- `hash_table.cpp`: C++ implementation.
- `output.txt`: Actual program output.
- `trace_report.md`: Manual trace and output comparison.
- `debugging_log.md`: Development and debugging records.

## Expected Learning Outcomes
1. Understand the Division Method of hashing.
2. Implement a hash table in C++.
3. Handle collisions using Linear Probing.
4. Compare manual calculations with actual program output.
5. Understand incremental project development.
## Algorithm

1. Initialize all hash table positions as empty.
2. Read the 20 personalized values.
3. Calculate the hash index using `key % 23`.
4. Check whether the calculated index is empty.
5. If occupied, use Linear Probing to find the next available position.
6. Insert the value into the available position.
7. Repeat until all values are inserted.
8. Display the final hash table.

## Compilation and Execution

Compile the program using:

bash
g++ hash_table.cpp -o hash_table

Execute the program:

bash
./hash_table

For Windows:

bash
hash_table.exe

## Time Complexity

- Average insertion: O(1), assuming a reasonable load factor.
- Worst-case insertion: O(n) due to linear probing.
- Display operation: O(m), where m is the table size.

## Final Result

The project demonstrates successful implementation of a hash table using the Division Method and Linear Probing with 20 personalized values.
