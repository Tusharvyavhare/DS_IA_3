# TRACE REPORT

## 1. Student Details
- PRN: 202602100010
- Subject: Data Structures
- Project: Hash Table Implementation
- Scenario: Mango Varieties

## 2. Personalized Dataset

Last four digits of PRN:

S = 10

Dataset formula:

v[i] = (S + 13 × i) mod 100

Personalized dataset:

10, 23, 36, 49, 62, 75, 88, 1, 14, 27, 40, 53, 66, 79, 92, 5, 18, 31, 44, 57

## 3. Hashing Technique

Division Method:

h(key) = key mod 23

Table size = 23 (chosen implementation assumption).

## 4. Collision Handling

Linear Probing is used to resolve collisions.

If a calculated index is already occupied, the next available index is checked.

Formula:

hᵢ(key) = (h(key) + i) mod 23

## 5. Manual Insertion Trace

| Key | Initial Index | Final Index |
|---:|---:|---:|
| 10 | 10 | 10 |
| 23 | 0 | 0 |
| 36 | 13 | 13 |
| 49 | 3 | 3 |
| 62 | 16 | 16 |
| 75 | 6 | 6 |
| 88 | 19 | 19 |
| 1 | 1 | 1 |
| 14 | 14 | 14 |
| 27 | 4 | 4 |
| 40 | 17 | 17 |
| 53 | 7 | 7 |
| 66 | 20 | 20 |
| 79 | 10 | 11 |
| 92 | 0 | 2 |
| 5 | 5 | 5 |
| 18 | 18 | 18 |
| 31 | 8 | 8 |
| 44 | 21 | 21 |
| 57 | 11 | 12 |

## 6. Final Hash Table

| Index | Value |
|---:|---:|
| 0 | 23 |
| 1 | 1 |
| 2 | 92 |
| 3 | 49 |
| 4 | 27 |
| 5 | 5 |
| 6 | 75 |
| 7 | 53 |
| 8 | 31 |
| 9 | EMPTY |
| 10 | 10 |
| 11 | 79 |
| 12 | 57 |
| 13 | 36 |
| 14 | 14 |
| 15 | EMPTY |
| 16 | 62 |
| 17 | 40 |
| 18 | 18 |
| 19 | 88 |
| 20 | 66 |
| 21 | 44 |
| 22 | EMPTY |

## 7. Trace-Match Report

The manually calculated final hash table was compared with the actual output produced by the C++ program.

The insertion positions and final table should match exactly.

## 8. Conclusion

The program successfully inserts all 20 personalized values into the hash table. The Division Method calculates the initial index, while Linear Probing resolves collisions by checking subsequent positions.