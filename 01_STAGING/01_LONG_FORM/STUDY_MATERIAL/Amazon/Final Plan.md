Of course. Here is a new plan structured precisely to your request, starting with your immediate next steps.

For the next 20 minutes, based on the frequency analysis of the provided lists, you will start with the most impactful topic: **Arrays**.

**14:00 - 14:20 →** Study problem **#560. Subarray Sum Equals K** (Array, Hash Table, Prefix Sum). Focus on how the use of a hash map to store prefix sums reduces the time complexity from a brute-force O(N^2) to an optimal O(N).

***

## 🚀 24-Hour High-Velocity Interview Plan

This plan is designed for rapid exposure to patterns, using your 10-15 minute per-problem strategy until your interview on Tuesday at 16:00.

### **Day 1: Monday Afternoon/Evening**

- [x] *16:20 - 18:00 + 20 →** Continue with top-frequency **Array & Hashing** problems.
    - [x] *16:20 - 16:40:** Study **#347. Top K Frequent Elements** (Array, Hash Table, Heap). Identify "Top K" as a primary indicator for using a Heap (Priority Queue).
    - [x] *16:40 - 17:00:** Study **#238. Product of Array Except Self** (Array, Prefix Sum). Focus on the clever O(1) space solution that uses prefix and postfix products.
    - [x] *17:00 - 17:20:** Study **#15. 3Sum** (Array, Two Pointers, Sorting). Recognize the pattern of sorting first, then using two pointers to find the remaining two numbers efficiently.
    - [x]  **17:20 - 17:40:** Study **#56. Merge Intervals** (Array, Sorting). Note that the key first step for almost all interval problems is sorting by the start time.
    - [x]  **17:40 - 18:00:** Study **#128. Longest Consecutive Sequence** (Array, Hash Table). Understand how a hash set provides O(1) lookups to check for the start of a sequence, leading to an O(N) solution.

- [x] *18:00 - 20:00 + 20 →** Shift to the next most frequent topic: **Graphs & Trees**.
    - [x]  **18:00 - 18:20:** Study **#200. Number of Islands** (Graph, BFS/DFS). Recognize that "connected components" on a grid is a classic graph traversal problem.
    - [x]  **18:20 - 18:40:** Study **#994. Rotting Oranges** (Graph, BFS). Identify "shortest time" or simultaneous expansion as a key indicator for BFS.
    - [x] *18:40 - 19:00:** Study **#236. Lowest Common Ancestor of a Binary Tree** (Tree, DFS). Understand the recursive DFS approach where you find the target nodes in the left and right subtrees.
    - [x] *19:00 - 19:20:** Study **#207. Course Schedule** (Graph, Topological Sort). See that "prerequisites" or dependencies indicate a directed graph and the need for topological sort to detect cycles.
    - [x] *19:20 - 19:40:** Study **#127. Word Ladder** (Graph, BFS). Learn to model the problem as a graph where words are nodes and an edge exists if they are one letter apart. "Shortest transformation" means BFS.
    - [x] *19:40 - 20:00:** Study **#210. Course Schedule II** (Graph, Topological Sort). This is a direct follow-up to Course Schedule I, where you return the sorted order itself.

- [ ] *20:00 - 21:00 + 20 →** Dedicate a full hour to **Behavioral Preparation**.
    - [ ] *20:00 - 20:30:** Brainstorm and create a "Story Bank" with 5-7 significant career situations.
    - [ ] *20:30 - 21:00:** Write out two of these stories using the **STAR method (Situation, Task, Action, Result)**, as this is strongly recommended by Amazon. Focus on quantifying the "Result" with metrics.

- [ ] *21:00 - 23:00 + 20 →** Focus on the next high-impact area: **Dynamic Programming**.
    - [ ] *21:00 - 21:20:** Study **#322. Coin Change** (DP). This is a classic "unbounded knapsack" type problem. Focus on the `dp[i]` state representing the minimum coins for amount `i`.
    - [ ] *21:20 - 21:40:** Study **#198. House Robber** (DP). Recognize the simple 1D DP pattern where the decision at house `i` depends on the outcomes at `i-1` and `i-2`.
    - [ ] *21:40 - 22:00:** Study **#5. Longest Palindromic Substring** (DP). Understand the `dp[i][j]` state representing if the substring from `i` to `j` is a palindrome.
    - [ ] *22:00 - 22:20:** Study **#300. Longest Increasing Subsequence** (DP). This is a fundamental DP pattern with an O(N^2) solution and a more clever O(N log N) solution using binary search.
    - [x] *22:20 - 22:40:** Study **#62. Unique Paths** (DP). See how this grid problem can be solved by defining `dp[i][j]` as the number of ways to reach cell `(i, j)`.

- [ ] *23:00 - 01:00 + 20 →** Cover **Linked Lists & Stacks**.
    - [x] *23:00 - 23:20:** Study **#146. LRU Cache** (Linked List, Hash Table). This is a critical design question. Understand the use of a hash map for O(1) lookups and a doubly-linked list for O(1) additions/removals.
    - [ ] *23:20 - 23:40:** Study **#23. Merge k Sorted Lists** (Linked List, Heap). Realize that merging more than two lists is a prime use case for a min-heap to efficiently track the smallest head node.
    - [x] *23:40 - 00:00:** Study **#739. Daily Temperatures** (Stack). Identify "next greater element" as the key pattern for a monotonic stack.
    - [x] *00:00 - 00:20:** Study **#84. Largest Rectangle in Histogram** (Stack). This is a hard but classic monotonic stack problem.
    - [ ] *00:20 - 00:40:** Study **#25. Reverse Nodes in k-Group** (Linked List, Recursion). This is an advanced pointer manipulation problem.

- [ ] *01:00 - Onwards →** **Rest**. Stop studying for the day to consolidate information.

### **Day 2: Tuesday Morning/Afternoon**

- [ ] *9:00 - 11:00 + 20 →** Begin with **Binary Search & Backtracking**.
    - [x] *9:00 - 9:20:** Study **#33. Search in Rotated Sorted Array** (Binary Search). Understand how to modify binary search to handle the pivot point.
    - [x] *9:20 - 9:40:** Study **#875. Koko Eating Bananas** (Binary Search). Recognize this as "Binary Search on the Answer," where you search for a feasible speed `k`.
    - [x] *9:40 - 10:00:** Study **#4. Median of Two Sorted Arrays** (Binary Search, Hard). This is a very challenging problem; focus on the high-level concept of partitioning the arrays.
    - [ ] *10:00 - 10:20:** Study **#79. Word Search** (Backtracking). This is a classic backtracking problem on a grid.
    - [ ] *10:20 - 10:40:** Study **#22. Generate Parentheses** (Backtracking). Understand the constraints (open < n, closed < open) that guide the backtracking recursion.
    - [ ] *10:40 - 11:00:** Study **#46. Permutations** (Backtracking). This is a fundamental backtracking template.

- [ ] *11:00 - 12:30 + 20 →** Final **Behavioral & Strategy** Session.
    - [x] *11:00 - 11:40:** **Map your STAR stories** to Amazon's 16 Leadership Principles.
    - [x] *11:40 - 12:10:** **Practice answers** for "Why Amazon?" and "Tell me about a time you failed." Remember to be specific for "Why Amazon?" and show what you learned from your failure.
    - [ ] *12:10 - 12:30:** **Prepare thoughtful questions** to ask your interviewers. Not having questions shows a lack of curiosity.

- [ ] *12:30 - 15:00 + 20 →** **Final High-Velocity Review**.
    - [ ] *12:30 - 13:30:** Rapidly review problems from the remaining topics: **Greedy, Intervals, and Design**.
        - [ ] `#55. Jump Game` (Greedy).
        - [ ] `#253. Meeting Rooms II` (Greedy, Heap, Intervals).
        - [ ] `#767. Reorganize String` (Greedy, Heap).
        - [ ] `#435. Non-overlapping Intervals` (Greedy, Intervals).
        - [x] `#295. Find Median from Data Stream` (Design, Heap).
    - [ ] *13:30 - 15:00:** Go through the **Top 10** problems from **Checklist 2** below one last time, verbally explaining the pattern of each to yourself.

- [ ] *15:00 →** **Stop all preparation.** Relax, eat a light meal, and get into a calm, confident headspace for your interview.

***

## Checklists for Your Sprint

### ✅ Checklist 1: Breadth & Foundational Problems

This list covers the fundamental patterns for each major topic.

* **Arrays & Hashing:** Two Sum, Contains Duplicate, Valid Anagram, Group Anagrams, Top K Frequent Elements, Product of Array Except Self, Valid Sudoku, Longest Consecutive Sequence, 3Sum, Container With Most Water, Best Time to Buy and Sell Stock.
* **Two Pointers / Sliding Window:** Valid Palindrome, Longest Substring Without Repeating Characters, Longest Repeating Character Replacement, Minimum Window Substring, Sliding Window Maximum.
* **Binary Search:** Binary Search, Search a 2D Matrix, Koko Eating Bananas, Find Minimum in Rotated Sorted Array, Search in Rotated Sorted Array, Median of Two Sorted Arrays.
* **Stack:** Valid Parentheses, Min Stack, Evaluate Reverse Polish Notation, Daily Temperatures, Largest Rectangle in Histogram.
* **Trees:** Invert Binary Tree, Maximum Depth of Binary Tree, Diameter of Binary Tree, Balanced Binary Tree, Same Tree, Subtree of Another Tree, Lowest Common Ancestor of a Binary Tree, Binary Tree Level Order Traversal, Validate Binary Search Tree, Kth Smallest Element in a BST, Construct Binary Tree from Preorder and Inorder Traversal.
* **Linked Lists:** Reverse Linked List, Merge Two Sorted Lists, Reorder List, Remove Nth Node From End of List, LRU Cache, Merge k Sorted Lists.
* **Graphs:** Number of Islands, Clone Graph, Rotting Oranges, Course Schedule, Pacific Atlantic Water Flow, Number of Provinces.
* **Heaps / Priority Queues:** Kth Largest Element in a Stream, K Closest Points to Origin, Kth Largest Element in an Array, Task Scheduler, Find Median from Data Stream.
* **Backtracking:** Subsets, Combination Sum, Permutations, Word Search, Palindrome Partitioning.
* **Dynamic Programming:** Climbing Stairs, House Robber, Coin Change, Longest Increasing Subsequence, Longest Common Subsequence, Word Break, Unique Paths.
* **Greedy:** Maximum Subarray, Jump Game, Gas Station, Partition Labels.
* **Intervals:** Insert Interval, Merge Intervals, Non-overlapping Intervals, Meeting Rooms II.
* **Tries:** Implement Trie (Prefix Tree), Design Add and Search Words Data Structure.

***

# LeetCode Interview Prep Checklist

## 📌 Topics & Problems  
**Mark as:** `- [ ]` (Pending) | `- [x]` (Done) | `- [/]` (In Progress)

### 1️⃣ Array & Hashing  
- [x] [347. Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements/)  
- [x] [238. Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self/)  
- [x] [15. 3Sum](https://leetcode.com/problems/3sum/)  
- [x] [56. Merge Intervals](https://leetcode.com/problems/merge-intervals/)  
- [x] [128. Longest Consecutive Sequence](https://leetcode.com/problems/longest-consecutive-sequence/)  

### 2️⃣ Graphs & Trees  
- [x] [200. Number of Islands](https://leetcode.com/problems/number-of-islands/)  
- [x] [994. Rotting Oranges](https://leetcode.com/problems/rotting-oranges/)  
- [x] [236. Lowest Common Ancestor](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree/)  
- [x] [207. Course Schedule](https://leetcode.com/problems/course-schedule/)  
- [x] [127. Word Ladder](https://leetcode.com/problems/word-ladder/)  
- [x] [210. Course Schedule II](https://leetcode.com/problems/course-schedule-ii/)  

### 3️⃣ Dynamic Programming  
- [ ] [322. Coin Change](https://leetcode.com/problems/coin-change/)  
- [ ] [198. House Robber](https://leetcode.com/problems/house-robber/)  
- [ ] [5. Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/)  
- [ ] [300. Longest Increasing Subsequence](https://leetcode.com/problems/longest-increasing-subsequence/)  
- [ ] [62. Unique Paths](https://leetcode.com/problems/unique-paths/)  

### 4️⃣ Linked Lists & Stacks  
- [x] [146. LRU Cache](https://leetcode.com/problems/lru-cache/)  
- [ ] [23. Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists/)  
- [x] [739. Daily Temperatures](https://leetcode.com/problems/daily-temperatures/)  
- [x] [84. Largest Rectangle in Histogram](https://leetcode.com/problems/largest-rectangle-in-histogram/)  
- [ ] [25. Reverse Nodes in k-Group](https://leetcode.com/problems/reverse-nodes-in-k-group/)  

### 5️⃣ Binary Search & Backtracking  
- [x] [33. Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array/)  
- [x] [875. Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas/)  
- [x] [4. Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays/)  
- [ ] [79. Word Search](https://leetcode.com/problems/word-search/)  
- [ ] [22. Generate Parentheses](https://leetcode.com/problems/generate-parentheses/)  
- [ ] [46. Permutations](https://leetcode.com/problems/permutations/)  

### 6️⃣ Greedy & Intervals  
- [x] [55. Jump Game](https://leetcode.com/problems/jump-game/)  
- [ ] [253. Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii/)  
- [ ] [767. Reorganize String](https://leetcode.com/problems/reorganize-string/)  
- [ ] [435. Non-overlapping Intervals](https://leetcode.com/problems/non-overlapping-intervals/)  
- [x] [295. Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream/)  

---

## 🔗 Obsidian Tips  
1. **Toggle Checkboxes**: Click checkboxes in **Preview mode** or use `Ctrl/Cmd + Click` in **Edit mode**.  
2. **Progress Tracking**: Use Dataview to count completed problems:  
     
   TABLE WITHOUT ID filter(file.tasks, (t) => t.completed).length AS Done  
   WHERE file.name = this.file.name  
3. **Link Previews**: Hover over problem links to see LeetCode descriptions (ensure **"Page Preview"** is enabled).  
### 🎯 Checklist 2: High-Frequency Amazon Questions (Combined & Prioritized)

#### **Arrays, Hashing & Strings**

- [ ] **#3. Longest Substring Without Repeating Characters (Medium):** A fundamental sliding window problem.
    
- [x] **#49. Group Anagrams (Medium):** Classic use of a hash map to group items by a computed key.
    
- [x] **#560. Subarray Sum Equals K (Medium):** An essential problem solved efficiently with a hash map and prefix sums.
    
- [ ] **#424. Longest Repeating Character Replacement (Medium):** An advanced sliding window problem.
    
- [ ] **#31. Next Permutation (Medium):** Tests careful in-place array manipulation and observation of patterns.
    
- [ ] **#53. Maximum Subarray (Medium):** A classic problem with both a greedy (Kadane's algorithm) and a DP solution.
    

#### **Two Pointers / Sliding Window**

- [ ] **#42. Trapping Rain Water (Hard):** A top-tier, challenging problem with multiple clever solutions (two-pointer, DP, stack).
    
- [ ] **#76. Minimum Window Substring (Hard):** The quintessential hard sliding window problem.
    
- [ ] **#11. Container With Most Water (Medium):** The canonical two-pointer problem.
    

#### **Linked Lists**

- [x] **#2. Add Two Numbers (Medium):** A fundamental linked list traversal and creation problem.
    
- [ ] **#138. Copy List with Random Pointer (Medium):** A very common question requiring a hash map to handle complex pointer copies.
    
- [ ] **#143. Reorder List (Medium):** A multi-step problem involving finding the midpoint, reversing a list, and merging.
    

#### **Design**

- [ ] **#155. Min Stack (Medium):** A classic design question for implementing a stack with O(1) min retrieval.
    
- [x] **#460. LFU Cache (Hard):** A more complex version of LRU Cache that is great for testing data structure design skills.
    
- [ ] **#380. Insert Delete GetRandom O(1) (Medium):** Requires combining a hash map and an array (or list) to achieve O(1) complexity.
    
- [ ] **#348. Design Tic-Tac-Toe (Medium):** A clever design problem that can be optimized to O(1) per move.
    

### **Tier 2: Broadening DSA Coverage**

#### **Graphs & Matrix Traversal**

- [ ] **#74. Search a 2D Matrix (Medium):** Tests applying binary search to a 2D structure.
    
- [x] **#48. Rotate Image (Medium):** A classic in-place matrix manipulation problem.
    
- [ ] **#133. Clone Graph (Medium):** A fundamental graph traversal problem using a hash map to track visited nodes.
    
- [ ] **#417. Pacific Atlantic Water Flow (Medium):** A great problem for practicing simultaneous graph traversals (BFS/DFS) from multiple sources.
    
- [x] **#695. Max Area of Island (Medium):** A direct follow-up to "Number of Islands," requiring you to track the size of each component.
    

#### **Binary Search**

- [ ] **#34. Find First and Last Position of Element in Sorted Array (Medium):** Requires modifying binary search to find boundaries.
    
- [ ] **#153. Find Minimum in Rotated Sorted Array (Medium):** A variation of "Search in Rotated Sorted Array" that focuses on finding the pivot point.
    
- [ ] **#1011. Capacity To Ship Packages Within D Days (Medium):** A prime example of "binary search on the answer."
    

#### **Trees**

- [ ] **#98. Validate Binary Search Tree (Medium):** A fundamental tree traversal problem with important constraints.
    
- [ ] **#199. Binary Tree Right Side View (Medium):** A great application of level-order traversal (BFS).
    
- [ ] **#105. Construct Binary Tree from Preorder and Inorder Traversal (Medium):** A classic recursive tree construction problem.
    
- [ ] **#230. Kth Smallest Element in a BST (Medium):** Best solved with an in-order traversal.
    

#### **Dynamic Programming**

- [ ] **#91. Decode Ways (Medium):** A classic 1D DP problem with string manipulation.
    
- [ ] **#45. Jump Game II (Medium):** A follow-up to "Jump Game" that can be solved with a greedy approach but has DP roots.
    
- [ ] **#518. Coin Change II (Medium):** The "unbounded knapsack" DP pattern, asking for combinations instead of permutations.
    

### **Tier 3: Important Variations & Hard Problems**

#### **Backtracking**

- [ ] **#39. Combination Sum (Medium):** A fundamental backtracking problem template.
    
- [ ] **#78. Subsets (Medium):** Another core backtracking pattern.
    
- [ ] **#51. N-Queens (Hard):** A classic and challenging backtracking problem.
    

#### **Stack**

- [ ] **#224. Basic Calculator (Hard):** A complex parsing problem elegantly solved with a stack.
    
- [ ] **#150. Evaluate Reverse Polish Notation (Medium):** A direct and fundamental application of a stack.
    

#### **Heaps (Priority Queues)**

- [ ] **#215. Kth Largest Element in an Array (Medium):** A problem that can be solved with sorting, quickselect, or a min-heap.
    
- [ ] **#621. Task Scheduler (Medium):** A problem where a greedy approach using a hash map or priority queue works well.
    

#### **Hard but Frequent**

- [ ] **#472. Concatenated Words (Hard):** A challenging problem combining string manipulation, DP, and often a Trie for optimization.
    
- [ ] **#212. Word Search II (Hard):** The advanced version of "Word Search" that is best solved by combining a Trie with backtracking.
    
- [ ] **#269. Alien Dictionary (Hard):** A unique problem that models characters as nodes in a graph to find a valid topological sort.


# Checklist 3 

* **Top Priority (From 30-day list):**
    - [ ]  `#3434. Maximum Frequency After Subarray Operation`
    - [ ]  `#3572. Maximize Y‑Sum by Picking a Triplet of Distinct X‑Values`
    * `#42. Trapping Rain Water`
    * `#1152. Analyze User Website Visit Pattern`
    * `#472. Concatenated Words`
    * `#875. Koko Eating Bananas`
    * `#323. Number of Connected Components in an Undirected Graph`
    * `#348. Design Tic-Tac-Toe`
    * `#2434. Using a Robot to Print the Lexicographically Smallest String`
    * `#51. N-Queens`
    * `#135. Candy`
    * `#212. Word Search II`
    * `#460. LFU Cache`
    * `#528. Random Pick with Weight`
    * `#1235. Maximum Profit in Job Scheduling`
    * `#2040. Kth Smallest Product of Two Sorted Arrays`
    * `#3234. Count the Number of Substrings With Dominant Ones`
    * `#32. Longest Valid Parentheses`
    * `#64. Minimum Path Sum`
    * `#72. Edit Distance`
    * `#269. Alien Dictionary`
    * `#399. Evaluate Division`
    * `#435. Non-overlapping Intervals`
    * `#540. Single Element in a Sorted Array`
    * `#827. Making A Large Island`
    * `#909. Snakes and Ladders`
    * `#1186. Maximum Subarray Sum with One Deletion`
    * `#1432. Max Difference You Can Get From Changing an Integer`
    * `#2115. Find All Possible Recipes from Given Supplies`
    * `#12. Integer to Roman`
    * `#25. Reverse Nodes in k-Group`
    * `#37. Sudoku Solver`
    * `#63. Unique Paths II`
    * `#77. Combinations`
    * `#85. Maximal Rectangle`
    * `#99. Recover Binary Search Tree`
    * `#120. Triangle`
    * `#130. Surrounded Regions`
    * `#140. Word Break II`
    * `#151. Reverse Words in a String`
    * `#227. Basic Calculator II`
    * `#304. Range Sum Query 2D - Immutable`
    * `#337. House Robber III`
    * `#465. Optimal Account Balancing`
    * `#518. Coin Change II`
    * `#692. Top K Frequent Words`
    * `#987. Vertical Order Traversal of a Binary Tree`
    * `#1032. Stream of Characters`
    * `#1061. Lexicographically Smallest Equivalent String`
    * `#1136. Parallel Courses`
    * `#1268. Search Suggestions System`
    * `#1482. Minimum Number of Days to Make m Bouquets`
    * `#1817. Finding the Users Active Minutes`
    * `#2055. Plates Between Candles`
    * `#2385. Amount of Time for Binary Tree to Be Infected`
    * `#3170. Lexicographically Minimum String After Removing Stars`
* **Next Priority (Unique problems from 6-month list, in order):**
    * `#767. Reorganize String`
    * `#735. Asteroid Collision`
    * `#122. Best Time to Buy and Sell Stock II`
    * `#2214. Minimum Health to Beat Game`
    * `#7. Reverse Integer`
    * `#3371. Identify the Largest Outlier in an Array`
    * `#443. String Compression`
    * `#102. Binary Tree Level Order Traversal`
    * `#103. Binary Tree Zigzag Level Order Traversal`
    * `#124. Binary Tree Maximum Path Sum`
    * `#863. All Nodes Distance K in Binary Tree`
    * `#71. Simplify Path`
    * `#297. Serialize and Deserialize Binary Tree`
    * `#973. K Closest Points to Origin`
    * `#1492. The kth Factor of n`
    * `#2551. Put Marbles in Bags`
    * `#189. Rotate Array`
    * `#273. Integer to English Words`
    * `#503. Next Greater Element II`
    * `#547. Number of Provinces`
    * `#907. Sum of Subarray Minimums`
    * `#6. Zigzag Conversion`
    * `#1650. Lowest Common Ancestor of a Binary Tree III`
    * `#10. Regular Expression Matching`
    * `#152. Maximum Product Subarray`
    * `#981. Time Based Key-Value Store`
    * `#1642. Furthest Building You Can Reach`
    * `#2170. Minimum Operations to Make the Array Alternating`
    * `#3462. Maximum Sum With at Most K Elements`
    * `#410. Split Array Largest Sum`
    * `#416. Partition Equal Subset Sum`
    * `#658. Find K Closest Elements`
    * `#787. Cheapest Flights Within K Stops`
    * `#134. Gas Station`
    * `#332. Reconstruct Itinerary`
    * `#636. Exclusive Time of Functions`
    * `#694. Number of Distinct Islands`
    * `#2221. Find Triangular Sum of an Array`
    * `#3455. Shortest Matching Substring`
    * `#3459. Length of Longest V-Shaped Diagonal Segment`
    * `#80. Remove Duplicates from Sorted Array II`
    * `#525. Contiguous Array`
    * `#632. Smallest Range Covering Elements from K Lists`
    * `#769. Max Chunks To Make Sorted`
    * `#904. Fruit Into Baskets`
    * `#2747. Count Zero Request Servers`
    * *...and so on for the rest of the 6-month list.*

***

## 📊 Most Impactful DSA Topics (Frequency Analysis)

Based on a combined analysis of the tags from both your 30-day and 6-month lists, here are the topics that appear most frequently. The plan is structured to prioritize these.

1.  **Array**
2.  **Dynamic Programming**
3.  **Hash Table**
4.  **String**
5.  **Greedy**
6.  **Sorting**
7.  **Depth-First Search (DFS)**
8.  **Breadth-First Search (BFS)**
9.  **Binary Search**
10. **Tree**
11. **Stack**
12. **Heap (Priority Queue)**
13. **Sliding Window**