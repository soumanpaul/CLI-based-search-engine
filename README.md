# CLI-Search-Engine 
- I'm building a system, and Datastructures and Algorithms are the tools I need to solve each engineering problem.



# Final Product

                 ┌─────────────────────┐
                 │     Documents       │
                 └──────────┬──────────┘
                            │
                            ▼
                    ┌───────────────┐
                    │    Crawler    │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │ Text Processor │
                    └───────┬───────┘
                            │
              ┌─────────────┼──────────────┐
              ▼             ▼              ▼
          HashTable       Trie          B+Tree
              │             │              │
              └─────────────┼──────────────┘
                            ▼
                     Search Engine
                            │
                            ▼
                    Ranking Engine
                            │
                 ┌──────────┴─────────┐
                 ▼                    ▼
             Heap/Top-K           Graph
                 │                    │
                 └──────────┬─────────┘
                            ▼
                    Recommendation
                            │
                            ▼
                    Optimization
                    /           \
                   /             \
                 DP          Approximation
                   \             /
                    \           /
                     Crawler
                         │
              ┌──────────┴──────────┐
              ▼                     ▼
          Bloom Filter             DSU
              │
              ▼
          LRU Cache
              │
              ▼
             RSA
              │
              ▼
       Quantum Experiments



# Roadmap
#	Milestone	                        Main DSA
1	Dynamic document store	             Array
2	Text tokenizer	                     String
3	Inverted index	                     Hash Table
4	Fast lookup	Binary                   Search
5	Result ordering	                     Sorting
6	Crawler	                             Queue / Stack
7	Index buckets	                     Linked List
8	Top-K search	                     Heap
9	Ordered index	                     BST
10	Autocomplete	                     Trie
11	Disk index	                         B/B+ Tree
12	Range analytics	                     Segment Tree
13	Prefix analytics	                 Fenwick Tree
14	Document relationships	             Graph
15	Search ranking	                     Graph + Heap
16	Parallel indexing	                 Divide & Conquer
17	Recommendation paths	             Recursion + Memoization
18	Reading planner	                     DP
19	Fast document selection	             Greedy
20	Document clusters	                 DSU
21	Permission system	                 Bit Manipulation
22	Query correction	                 Backtracking
23	Search optimization	                 Branch & Bound
24	Resource allocation	                 Linear Programming
25	Large-scale optimization	         Approximation
26	Fast duplicate detection	         Bloom Filter
27	Query acceleration	                 LRU Cache
28	Secure documents	                 RSA
29	Quantum search lab	                 Quantum Algorithms
30	Productionization	                 All combined



## Trie

### Why does the product need it?

Autocomplete.

### Naive solution

Scan every known word.

Complexity:
O(N * L)

### Better solution

Trie.

### Operations

insert()
search()
starts_with()

### Complexity

insert: O(L)
search: O(L)
prefix: O(L)

### Memory tradeoff

...

### Implementation

...

### Benchmark

...

### Product integration

src/search/autocomplete.py

### What I learned

...
