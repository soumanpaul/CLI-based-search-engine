
# Milestone 20 — Disjoint Set / Union-Find
- Your crawler discovers:
websites
documents
communities

- You want to determine which documents belong to the same connected cluster.

# Implement:
DisjointSet

# with:
find()
union()
path_compression
union_by_rank


# Then use it for:
- document clustering


# Milestone 21 — Bit Manipulation
- Introduce compact representations.
- For example: Document permissions

# Represent:
READ
WRITE
ADMIN
PUBLIC
ARCHIVED

# using bits.
00001 = READ
00010 = WRITE
00100 = ADMIN
01000 = PUBLIC
10000 = ARCHIVED

# Then:
permissions & READ
permissions | WRITE
permissions ^ ...

- You'll learn bit operations through an actual feature

# Milestone 22 — Backtracking
- Build: Search query correction

- Given:
"algoritm"

# generate candidate corrections:
algorithm
algorithmic
algorithms
- You can model candidate generation as a search tree


# Implement:
- backtracking() with pruning.


# Milestone 23 — Branch and Bound
- Now make recommendation/search optimization harder.
- Suppose: 1,000 documents
- You want the best combination under several constraints

- Brute force:
2^N
is impossible

- `Build a branch-and-bound solver`

# Compare:
- brute force
- backtracking
- branch and bound

- This is a great project milestone because you can visually demonstrate how pruning reduces the search space.

