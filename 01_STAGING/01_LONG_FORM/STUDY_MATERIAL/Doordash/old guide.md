Of course. Here is the same high-intensity study plan, broken down with specific time slots for each problem. The pace is aggressive, so stick to the schedule to cover all the key patterns.

### **Saturday Afternoon/Evening (2:50 PM - 9:50 PM)**

#### **Session 1: Graph & Matrix Traversal (3:00 PM - 6:20 PM)**

_Goal: Master BFS for shortest paths and DFS for connectivity._

- [x] **3:00 PM - 3:15 PM:** **#200. Number of Islands (Medium):** (Warm-up) Focus on the standard DFS grid traversal to "sink" an island.
    
- [x] **3:15 PM - 3:40 PM:** **#286. Walls and Gates (Medium):** Understand the multi-source BFS pattern; initialize the queue with all gates.
    
- [x] **3:40 PM - 4:05 PM:** **#695. Max Area of Island (Medium):** Adapt your DFS from the warm-up to return the size of each island.
    
- [ ] **4:05 PM - 4:35 PM:** **#317. Shortest Distance from All Buildings (Hard):** Grasp the concept of running a separate BFS from each building and accumulating distances.
    
- [x] **4:35 PM - 5:00 PM:** **#207. Course Schedule (Medium):** Focus on the topological sort pattern using DFS and three states (visiting, visited, unvisited) to detect cycles.
    
- [x] **5:00 PM - 5:25 PM:** **#210. Course Schedule II (Medium):** Modify the previous problem to store and return the topological order.
    
- [ ] **5:25 PM - 5:50 PM:** **#133. Clone Graph (Medium):** Understand the use of a hash map to store created nodes and prevent infinite loops during traversal.
    
- [x] **5:50 PM - 6:20 PM:** **#827. Making A Large Island (Hard):** Review the two-pass approach: first, use DFS to find and label all islands with their sizes. Second, iterate through '0's to find the best merge.
    

---

#### **Session 2: Trees & Recursion (6:20 PM - 9:50 PM)**

_Goal: Solidify tree traversals, path-finding, and Trie-based design._

- [x] **6:20 PM - 6:40 PM:** **#236. Lowest Common Ancestor of a Binary Tree (Medium):** (Warm-up) Understand the recursive solution where you find nodes in left/right subtrees.
    
- [ ] **6:40 PM - 7:10 PM:** **#124. Binary Tree Maximum Path Sum (Hard):** The key is a recursive function that returns the "max path _ending_ at the current node" while updating a global max.
    
- [ ] **7:10 PM - 7:40 PM:** **#297. Serialize and Deserialize Binary Tree (Hard):** Focus on the pre-order traversal approach for serialization and the corresponding recursive method for deserialization.
    
- [ ] **7:40 PM - 8:10 PM:** **#987. Vertical Order Traversal of a Binary Tree (Hard):** Review the BFS with coordinate tracking (row, col) and the sorting logic for the final output.
    

**_(8:10 PM - 9:00 PM: Dinner & Mental Break)_**

- [ ] **9:00 PM - 9:25 PM:** **#208. Implement Trie (Prefix Tree) (Medium):** Focus on the node structure (children map + isEndOfWord boolean).
    
- [ ] **9:25 PM - 9:50 PM:** **#1268. Search Suggestions System (Medium):** See how to apply your Trie structure to find all words with a given prefix.
    

---

### **Saturday Night (9:50 PM - 2:00 AM)**

#### **Session 3: Dynamic Programming (9:50 PM - 11:50 PM)**

_Goal: Recognize the most common DP patterns._

- [ ] **9:50 PM - 10:05 PM:** **#198. House Robber (Medium):** (Warm-up) The classic `dp[i] = max(dp[i-1], dp[i-2] + nums[i])` recurrence.
    
- [ ] **10:05 PM - 10:30 PM:** **#322. Coin Change (Medium):** Understand the 1D DP "unbounded knapsack" approach.
    
- [ ] **10:30 PM - 10:55 PM:** **#1143. Longest Common Subsequence (Medium):** The most fundamental 2D DP pattern.
    
- [ ] **10:55 PM - 11:20 PM:** **#5. Longest Palindromic Substring (Medium):** Review the 2D DP approach where `dp[i][j]` depends on the inner substring.
    
- [ ] **11:20 PM - 11:50 PM:** **#139. Word Break (Medium):** Understand the 1D DP where `dp[i]` represents if the string up to index `i` is breakable.
    

---

#### **Session 4: Arrays, Intervals & Sliding Window (11:50 PM - 2:00 AM)**

_Goal: Master two-pointers, prefix sums, and interval management._

- [ ] **11:50 PM - 12:10 AM:** **#56. Merge Intervals (Medium):** The key is sorting by the start time.
    
- [ ] **12:10 AM - 12:30 AM:** **#3. Longest Substring Without Repeating Characters (Medium):** Review the classic sliding window with a hash set/map.
    
- [ ] **12:30 AM - 12:55 AM:** **#560. Subarray Sum Equals K (Medium):** The essential prefix sum + hash map pattern.
    
- [ ] **12:55 AM - 1:20 AM:** **#42. Trapping Rain Water (Hard):** Focus on understanding the logic behind the optimal two-pointer solution.
    
- [ ] **1:20 AM - 1:40 AM:** **#239. Sliding Window Maximum (Hard):** Review how a Deque is used to maintain the max element in O(1) time for the window.
    
- [ ] **1:40 AM - 2:00 AM:** **#76. Minimum Window Substring (Hard):** Review the two-pointer and hash map template for this classic problem.
    

---

## **SLEEP (2:00 AM - 7:00 AM)**

### **Sunday Morning (7:00 AM - 11:50 AM)**

#### **Session 5: Heaps & Stacks (7:00 AM - 9:20 AM)**

_Goal: Review "Top K" patterns (Heaps) and parsing/monotonic patterns (Stacks)._

- [ ] **7:00 AM - 7:20 AM:** **#215. Kth Largest Element in an Array (Medium):** Use a min-heap of size K.
    
- [ ] **7:20 AM - 7:45 AM:** **#1834. Single-Threaded CPU (Medium):** The quintessential heap-based scheduling problem.
    
- [ ] **7:45 AM - 8:15 AM:** **#295. Find Median from Data Stream (Hard):** The famous two-heap (max-heap, min-heap) design pattern.
    
- [ ] **8:15 AM - 8:35 AM:** **#23. Merge k Sorted Lists (Hard):** The canonical use case for a min-heap.
    
- [ ] **8:35 AM - 8:55 AM:** **#739. Daily Temperatures (Medium):** The classic monotonic stack problem.
    
- [ ] **8:55 AM - 9:20 AM:** **#84. Largest Rectangle in Histogram (Hard):** The most famous hard monotonic stack problem.
    

---

#### **Session 6: Binary Search & Design (9:20 AM - 11:20 AM)**

_Goal: Master "binary search on the answer" and review key design questions._

- [ ] **9:20 AM - 9:40 AM:** **#33. Search in Rotated Sorted Array (Medium):** The most common variation of standard binary search.
    
- [ ] **9:40 AM - 10:00 AM:** **#875. Koko Eating Bananas (Medium):** The perfect introduction to "binary search on the answer."
    
- [ ] **10:00 AM - 10:25 AM:** **#4. Median of Two Sorted Arrays (Hard):** Briefly review the high-level concept of partitioning the arrays via binary search.
    
- [ ] **10:25 AM - 10:55 AM:** **#146. LRU Cache (Medium):** Must-know design question using a hash map and a doubly-linked list.
    
- [ ] **10:55 AM - 11:20 AM:** **#380. Insert Delete GetRandom O(1) (Medium):** Understand the hash map + array combination for O(1) operations.
    

---

#### **Final Lap: High-Value Review (11:20 AM - 11:50 AM)**

_Quickly re-read the solutions for these key hard problems to refresh the patterns._

- [ ] **11:20 AM - 11:30 AM:** **#25. Reverse Nodes in k-Group (Hard):** Review recursive pointer manipulation.
    
- [ ] **11:30 AM - 11:40 AM:** **#269. Alien Dictionary (Hard):** Refresh your memory on building a graph from rules and finding the topological sort.
    
- [ ] **11:40 AM - 11:50 AM:** **#41. First Missing Positive (Hard):** Review the trick of using the array itself as a hash map.


### **Schedule Overview**

- **Start:** Sunday, 3:30 PM
    
- **Sleep:** 1:00 AM - 8:00 AM (7 hours)
    
- **End:** Monday, 3:30 PM
    

---

### **Sunday Afternoon (3:30 PM - 7:30 PM)**

#### **Session 1: Foundational Patterns & Easy Warm-ups (1 Hour)**

_Goal: Build momentum and cover basic patterns._

- [x] **3:30 PM - 3:45 PM:** **#1. Two Sum (Easy):** The most classic use of a hash map for O(1) lookups.
    
- [x] **3:45 PM - 4:00 PM:** **#1790. Check if One String Swap Can Make Strings Equal (Easy):** Focus on edge cases and clean conditional logic.
    
- [ ] **4:00 PM - 4:15 PM:** **#859. Buddy Strings (Easy):** Similar to the above, a good problem for careful case analysis.
    
- [ ] **4:15 PM - 4:30 PM:** **#2185. Counting Words With a Given Prefix (Easy):** A straightforward problem to warm up string manipulation.
    

#### **Session 2: Core Graph, Matrix & Heap Problems (3 Hours)**

_Goal: Tackle the most common problem types on the list._

- [ ] **4:30 PM - 5:00 PM:** **#329. Longest Increasing Path in a Matrix (Hard):** The core pattern is DFS with memoization (a form of DP) to avoid re-computing paths.
    
- [ ] **5:00 PM - 5:25 PM:** **#542. 01 Matrix (Medium):** A classic multi-source BFS problem. Start BFS from all '0' cells simultaneously.
    
- [ ] **5:25 PM - 5:55 PM:** **#778. Swim in Rising Water (Hard):** This can be solved with a modification of Dijkstra's algorithm, using a min-heap to always explore the path with the lowest "water level."
    
- [ ] **5:55 PM - 6:20 PM:** **#621. Task Scheduler (Medium):** A greedy problem. Understand the formula-based solution and the priority queue/hash map approach.
    
- [ ] **6:20 PM - 6:45 PM:** **#826. Most Profit Assigning Work (Medium):** A greedy problem that becomes simple after sorting both jobs and workers.
    
- [ ] **6:45 PM - 7:10 PM:** **#1383. Maximum Performance of a Team (Hard):** A tricky greedy problem where you sort by one metric (efficiency) and use a min-heap to maintain the best of another (speed).
    
- [ ] **7:10 PM - 7:30 PM:** **#547. Number of Provinces (Medium):** A great problem to practice either DFS, BFS, or the Union-Find data structure to count connected components.
    

---

## **_(7:30 PM - 8:30 PM: Dinner Break)_**

### **Sunday Evening (8:30 PM - 1:00 AM)**

#### **Session 3: Design, Tries & Advanced Trees (2.5 Hours)**

_Goal: Focus on "design" questions, which often involve combining data structures like Tries._

- [ ] **8:30 PM - 9:00 PM:** **#588. Design In-Memory File System (Hard):** Understand how a Trie is the perfect data structure for representing the file path hierarchy.
    
- [ ] **9:00 PM - 9:25 PM:** **#211. Design Add and Search Words Data Structure (Medium):** A variation of a Trie that needs a recursive search function to handle the '.' wildcard.
    
- [ ] **9:25 PM - 9:50 PM:** **#642. Design Search Autocomplete System (Hard):** Combines a Trie for prefix searching with logic to store and sort results.
    
- [ ] **9:50 PM - 10:15 PM:** **#1804. Implement Trie II (Prefix Tree) (Medium):** An extension of the basic Trie that requires tracking counts for both full words and prefixes.
    
- [ ] **10:15 PM - 10:40 PM:** **#1472. Design Browser History (Medium):** This is commonly solved using two stacks or a dynamic array/list with a pointer.
    
- [ ] **10:40 PM - 11:00 PM:** **#2049. Count Nodes With the Highest Score (Medium):** A tree traversal (post-order DFS) problem where you need to calculate subtree sizes to find the score.
    

#### **Session 4: Hard Applications & Parsing (2 Hours)**

_Goal: Review complex problems that often involve parsing or advanced combinations of data structures._

- [ ] **11:00 PM - 11:30 PM:** **#772. Basic Calculator III (Hard):** This requires two stacks (one for operands, one for operators) and a solid understanding of the shunting-yard algorithm concept to handle order of operations and parentheses.
    
- [ ] **11:30 PM - 12:00 AM:** **#212. Word Search II (Hard):** The optimal solution combines a Trie (built from the dictionary words) with a backtracking DFS on the grid. This avoids repeatedly searching for words.
    
- [ ] **12:00 AM - 12:30 AM:** **#37. Sudoku Solver (Hard):** A classic backtracking problem. Focus on the recursive structure: try a number, recurse, and backtrack if it fails.
    
- [ ] **12:30 AM - 1:00 AM:** **#1359. Count All Valid Pickup and Delivery Options (Hard):** This is a combinatorics and math problem. Understand the logic of calculating the available slots at each step.
    

---

## **_(1:00 AM - 8:00 AM: Sleep)_**

### **Monday Morning (8:30 AM - 12:30 PM)**

#### **Session 5: Core DP & Array/String Logic (2 Hours)**

_Goal: Refresh DP patterns and common array/string manipulations._

- [ ] **8:30 AM - 9:00 AM:** **#1235. Maximum Profit in Job Scheduling (Hard):** A classic dynamic programming problem. The key is to sort by end times and use binary search (or a heap) to find the latest non-conflicting job.
    
- [ ] **9:00 AM - 9:25 AM:** **#55. Jump Game (Medium):** A classic greedy problem where you keep track of the `max_reach` possible from your current position.
    
- [ ] **9:25 AM - 9:50 AM:** **#45. Jump Game II (Medium):** A slightly harder version of Jump Game that tracks the end of the current "jump level."
    
- [ ] **9:50 AM - 10:10 AM:** **#31. Next Permutation (Medium):** Review the specific, elegant algorithm for finding the next lexicographical permutation in-place.
    
- [ ] **10:10 AM - 10:30 AM:** **#49. Group Anagrams (Medium):** The core idea is to use a hash map where the key is the sorted version of the string.
    

#### **Session 6: Sliding Window & Subarray Problems (2 Hours)**

_Goal: Focus on window-based problems and prefix sum techniques._

- [ ] **10:30 AM - 10:55 AM:** **#209. Minimum Size Subarray Sum (Medium):** A classic sliding window problem with two pointers.
    
- [ ] **10:55 AM - 11:20 AM:** **#304. Range Sum Query 2D - Immutable (Medium):** Understand how to build a 2D prefix sum array (or summed-area table) for O(1) query time.
    
- [ ] **11:20 AM - 11:45 AM:** **#480. Sliding Window Median (Hard):** The optimal solution uses two heaps (a max-heap and a min-heap) to keep track of the two halves of the window, similar to "Find Median from Data Stream."
    
- [ ] **11:45 AM - 12:10 PM:** **#1152. Analyze User Website Visit Pattern (Medium):** A combination of data processing (using hash maps) and generating all possible 3-sequence patterns.
    
- [ ] **12:10 PM - 12:30 PM:** **#18. 4Sum (Medium):** Understand how to generalize the 3Sum problem by adding another loop and handling duplicates carefully.
    

---

## **_(12:30 PM - 1:15 PM: Lunch Break)_**

### **Monday Afternoon (1:15 PM - 3:30 PM)**

#### **Session 7: Final Polish & Special Topics (2.25 Hours)**

_Goal: Quickly review remaining high-value problems and patterns._

- [ ] **1:15 PM - 1:40 PM:** **#1944. Number of Visible People in a Queue (Hard):** A tricky but excellent problem for the monotonic stack pattern.
    
- [ ] **1:40 PM - 2:00 PM:** **#1011. Capacity To Ship Packages Within D Days (Medium):** A perfect example of "Binary Search on the Answer."
    
- [ ] **2:00 PM - 2:20 PM:** **#347. Top K Frequent Elements (Medium):** A classic "Top K" problem solvable with a hash map and a min-heap or by using the Quickselect algorithm.
    
- [ ] **2:20 PM - 2:40 PM:** **#759. Employee Free Time (Hard):** This is an interval problem. The key is to flatten all intervals into a single list, sort them, and then find the gaps.
    
- [ ] **2:40 PM - 3:00 PM:** **#277. Find the Celebrity (Medium):** A logic puzzle that can be solved in O(n) by eliminating non-celebrities in a first pass and verifying the candidate in a second pass.
    
- [ ] **3:00 PM - 3:30 PM:** **Final Review:** Quickly re-read the solutions for 2-3 of the hardest or most interesting problems you've covered (e.g., **#329, #588, #772**) to solidify the patterns in your mind.