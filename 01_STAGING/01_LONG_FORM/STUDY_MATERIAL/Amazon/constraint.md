Here’s a structured table summarizing the problems, their key techniques, constraints, and complexities:  

| Problem # | Problem Name                       | Data Structure / Algorithm     | Constraint                     | Time Complexity | Space Complexity |
| --------- | ---------------------------------- | ------------------------------ | ------------------------------ | --------------- | ---------------- |
| 1         | Two Sum                            | Hash Map                       | `n ≤ 10⁴`                      | O(n)            | O(n)             |
| 15        | 3Sum                               | Sorting + Two Pointers         | `n ≤ 3000`                     | O(n²)           | O(1)             |
| 36        | Valid Sudoku                       | Hash Set                       | Fixed 9×9 grid                 | O(1)            | O(1)             |
| 48        | Rotate Image                       | Matrix Manipulation            | `n ≤ 20`                       | O(n²)           | O(1)             |
| 49        | Group Anagrams                     | Hash Map (+ Sorting/Counting)  | `n ≤ 10⁴` strings              | O(n × k)        | O(n × k)         |
| 62        | Unique Paths                       | Dynamic Programming            | `m, n ≤ 100`                   | O(m × n)        | O(min(m, n))     |
| 72        | Edit Distance                      | Dynamic Programming            | `m, n ≤ 500`                   | O(m × n)        | O(min(m, n))     |
| 121       | Best Time to Buy/Sell Stock        | One-Pass Traversal             | `n ≤ 10⁵`                      | O(n)            | O(1)             |
| 125       | Valid Palindrome                   | Two Pointers                   | `n ≤ 2×10⁵`                    | O(n)            | O(1)             |
| 146       | LRU Cache                          | Hash Map + Doubly Linked List  | `capacity ≤ 3000`              | O(1)            | O(capacity)      |
| 200       | Number of Islands                  | DFS/BFS                        | `m, n ≤ 300`                   | O(m × n)        | O(m × n)         |
| 217       | Contains Duplicate                 | Hash Set                       | `n ≤ 10⁵`                      | O(n)            | O(n)             |
| 219       | Contains Duplicate II              | Hash Map / Sliding Window      | `n ≤ 10⁵`                      | O(n)            | O(min(n, k))     |
| 238       | Product of Array Except Self       | Prefix/Suffix Products         | `n ≤ 10⁵`                      | O(n)            | O(1)             |
| 242       | Valid Anagram                      | Hash Map (Frequency) / Sorting | `n ≤ 5×10⁴`                    | O(n)            | O(1)             |
| 271       | Encode and Decode Strings          | String Serialization           | `n ≤ 200` strings, `len ≤ 200` | O(N)            | O(N)             |
| 347       | Top K Frequent Elements            | Hash Map + Bucket Sort         | `n ≤ 10⁵`                      | O(n)            | O(n)             |
| 460       | LFU Cache                          | Hash Maps + Doubly Linked List | `capacity ≤ 10⁴`               | O(1)            | O(capacity)      |
| 560       | Subarray Sum Equals K              | Prefix Sum + Hash Map          | `n ≤ 2×10⁴`                    | O(n)            | O(n)             |
| 695       | Max Area of Island                 | DFS/BFS                        | `m, n ≤ 50`                    | O(m × n)        | O(m × n)         |
| 904       | Fruit Into Baskets                 | Sliding Window                 | `n ≤ 10⁵`                      | O(n)            | O(1)             |
| 1152      | Analyze User Website Visit Pattern | Hash Map + Combinatorics       | `n ≤ 50` logs                  | O(N × L³)       | O(P)             |
| 1834      | Single-Threaded CPU                | Min-Heap + Sorting             | `n ≤ 10⁵`                      | O(n log n)      | O(n)             |
| 2357      | Make Array Zero by Subtracting     | Hash Set                       | `n ≤ 100`                      | O(n)            | O(n)             |
| 3438      | Find Valid Pair of Adjacent Digits | Hash Map (Frequency Count)     | `n ≤ 100`                      | O(n)            | O(1)             |
| 3477      | Fruits Into Baskets II             | Brute Force Simulation         | `n ≤ 100`                      | O(n²)           | O(n)             |
| 3479      | Fruits Into Baskets III            | Segment Tree                   | `n ≤ 10⁵`                      | O(n log n)      | O(n)             |
|           |                                    |                                |                                |                 |                  |
|           |                                    |                                |                                |                 |                  |
|           |                                    |                                |                                |                 |                  |
|           |                                    |                                |                                |                 |                  |
|           |                                    |                                |                                |                 |                  |
|           |                                    |                                |                                |                 |                  |

### **Key Notes:**
- **`k`** in **Group Anagrams (49)** = **max string length** (not average).  
- **`N`** in **Encode/Decode Strings (271)** = **total characters across all strings**.  
- **`L`** in **Analyze User Visit Pattern (1152)** = **max visits per user**.  
- **`P`** in **1152** = **number of unique 3-sequence patterns**.  

This table provides a quick reference for time/space complexities and constraints. Let me know if you'd like any refinements! 🚀