# Amazon SDE Interview Preparation Guide
#tags: #interview-prep #amazon #sde #guide #behavioral #system-design

## 🧭 Role Overview: Software Development Engineer (SDE)
Amazon SDEs are expected to own the entire software development lifecycle, deliver scalable solutions, and demonstrate strong CS fundamentals.

## 🧠 Interview Structure (60 Minutes)
| Segment | Duration | Focus |
|---|---|---|
| 👋 Introduction | 5 mins | Rapport, background, logistics |
| 🧑‍💻 Coding | 30 mins | One algorithm problem (real code) |
| 🎙️ Behavioral (LPs) | 20 mins | STAR format answers for Leadership Principles |
| ❓ Candidate Questions | 5 mins | Your chance to ask thoughtful questions |

*Source:*

## 💻 Technical Preparation

### 1. Data Structures
- **Must Understand**: Arrays, Strings, Linked Lists, Hash Maps, Trees, Tries, Heaps, Graphs, Stacks, Queues.
- **Know Tradeoffs**: Time/space complexity, lookup/update performance.

### 2. Algorithms
- **Must Practice**: Sorting, Searching (BFS, DFS), Recursion, Backtracking, Greedy, Two Pointers, Sliding Window, Dynamic Programming, Graph algorithms (Dijkstra, Union-Find).

### 3. Coding Execution
- Practice **whiteboard-style coding** (no compiler).
- Write **production-ready code**: good naming, modularity, error handling.
- **Communicate** your thought process clearly.

### Study Material: 
- ![[05_RESOURCES/Articles_and_PDFs/Amazon/Ace Amazon SDE - 1.pdf]]
- ![[05_RESOURCES/Articles_and_PDFs/Amazon/SDE Onsite Competency Prep Guide.pdf]]

## 🏗️ System Design Preparation

### Key Expectations
- Design for: **Scalability, High Availability, Resilience, Security, Cost-efficiency**.

### Common Components
- Load Balancers, DNS, REST APIs, Caching Layers (Redis), Message Queues (Kafka, SQS), Databases (SQL vs. NoSQL), CDNs.

### Design Process
1.  **Clarify Requirements**: Functional and non-functional needs.
2.  **Define High-Level Architecture**: Client → LB → App Servers → DB/Cache.
3.  **Discuss Core Components**: APIs, Databases, Cache.
4.  **Handle Scale and Failure**: Redundancy, failover, replication.
5.  **Analyze Tradeoffs**: Latency vs. throughput, CAP Theorem.

### Study Material: 
- ![[05_RESOURCES/Articles_and_PDFs/Amazon/Amazon Systems Design Preparation.pdf]]

## 👑 Amazon Leadership Principles (LPs)
Amazon evaluates behavioral fit using **16 Leadership Principles**. You must answer using the **STAR** format.

### STAR Format
-   **S**ituation – Context and background
-   **T**ask – Your responsibility
-   **A**ction – Steps you personally took
-   **R**esult – Outcome with **metrics** and **lessons learned**

### Key Leadership Principles
- Customer Obsession
- Ownership
- Invent and Simplify
- Are Right, A Lot
- Learn and Be Curious
- Insist on the Highest Standards
- Think Big
- Bias for Action
- Earn Trust
- Dive Deep
- Have Backbone; Disagree and Commit
- Deliver Results

### Prep Strategy
- Prepare **10-15 professional stories**.
- Map each story to **1-2 leadership principles**.
- Prioritize recent and diverse examples.
- Clarify **your personal role** in team achievements.

### Practice Guides:
- ![[05_RESOURCES/Articles_and_PDFs/Amazon/Fortify-Experts-Behavioral-Questions-Based-on-Amazon-Principles.pdf]]
- ![[05_RESOURCES/Articles_and_PDFs/Amazon/STAR Leadership Principals.pdf]]