# COURSE 3 — Divide & Conquer / Greedy / DP
- This is where the project becomes much more algorithmically interesting

# Milestone 16 — Divide and Conquer
- Suppose you have millions of documents. You want to process them in parallel.

# Split:
Documents
   ↓
┌───────┬───────┬───────┬───────┐
│ chunk │ chunk │ chunk │ chunk │
└───────┴───────┴───────┴───────┘
    ↓       ↓       ↓       ↓
 index   index   index   index
    └───────┬───────┘
            ↓
          merge

# Implement:
- parallel_index() This gives you a practical reason to understand divide-and-conquer.


# Milestone 17 — Recursion + Memoization
- Recommendation problem: Given a document, find the best sequence of related documents to read.

- Simplified: A → B → C → D
But there may be many possible paths.

- Build a recursive recommendation/path algorithm.
- Then introduce: memoization

# and compare:
naive recursion
vs
memoization
- Measure the difference.


# Milestone 18 — Dynamic Programming
- Create a feature: "Find the most valuable sequence of documents under a reading-time budget."

# User has 30 minutes.
Document       Time     Value
--------------------------------
A               5        8
B              10       15
C               7       10
D              20       30

# Now you're basically solving a variation of:
- 0/1 Knapsack

# Implement:
- recursive
- recursive + memoization
- bottom-up DP

- Compare all three.

- This is a fantastic way to actually learn DP

# Milestone 19 — Greedy
- Build: "Select the most useful documents under a limited processing budget."

- Try:
highest score first
score / cost
- Then compare your greedy solution against DP on small datasets.
- Now you learn an extremely important lesson:
- Greedy algorithms can be fast without necessarily producing the optimal solution.










