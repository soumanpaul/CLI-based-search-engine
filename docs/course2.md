# COURSE 2 CHECKPOINT

                         ┌── Trie
                         │
Query → Parser → Index ──┼── B+Tree
                         │
                         └── Hash Table
                              │
                              ▼
                           Ranking
                              │
                              ▼
                         Top-K Heap
                              │
                              ▼
                         Search Results

Documents → Graph → Related Documents

# COURSE 2 — Trees + Graphs
- Now things get much more interesting.

# Milestone 9 — BST
- Problem: Search terms need to be maintained in sorted order.

- Build:
BinarySearchTree

- Support:
insert
delete
search
min
max
predecessor
successor
inorder

# Then compare:
HashTable
BST
Sorted Array
- for different workloads.

# Milestone 10 — Trie
- Product requirement: "As the user types alg..., show suggestions."
- Now you need a Trie.

# Example:

                 root
                  |
                  a
                  |
                  l
                /   \
               g     l
               |
               o
               |
               r

# Implement:
insert(word)
search(word)
starts_with(prefix)
autocomplete(prefix)

# Then:
GET /autocomplete?q=alg

# returns:
algorithm
algorithmic
algorithms
algorithm design

# Milestone 11 — B-Tree / B+Tree
- Now imagine: 10 million documents
- Your in-memory structures aren't enough. You need disk-friendly indexing.

# This is where:
B-Tree
B+Tree
become meaningful.
- Build a simplified B+Tree

# Use it for:
document_id → document metadata

# Study:
disk pages
fanout
node splitting
range queries

- You don't need to build production-grade storage.
- The educational goal is understanding why databases use B-Trees/B+Trees

# Milestone 12 — Segment Tree
- Now introduce analytics.
- Your search system records:
timestamp
query
number_of_results
latency
clicks

- You want: "How many searches occurred between 10:00 and 12:00?"
- Implement a Segment Tree.
# Then support:
range_sum()
range_min()
range_max()

- This connects a textbook structure to analytics.


# Milestone 13 — Fenwick Tree
- Now track cumulative statistics.
- Example: hour → searches

- Use a Binary Indexed Tree/Fenwick Tree for:
    prefix_sum()
    update()

- Compare:
Naive
Segment Tree
Fenwick Tree
- and document when each is appropriate.

# Milestone 14 — Graph
- Now your documents become connected.

# Example:
- Machine Learning
      |
      ├── Neural Networks
      |
      ├── Statistics
      |
      └── Optimization

- Create: DocumentGraph

- where:
node = document
edge = relationship

- Implement:
BFS
DFS
connected components
shortest path

# Milestone 15 — Search Ranking
- Now you're no longer simply matching words.

# You need:
query
 ↓
candidate documents
 ↓
ranking
 ↓
top results

# Start with simple scoring:
score =
    term_frequency
    + title_match
    + phrase_match
    + popularity

- Then build toward: TF-IDF and eventually: BM25
- This becomes your first serious ranking system.

