
# COURSE 6 — Advanced DS + RSA + Quantum
- This becomes the final layer.

# Milestone 26 — Advanced Data Structures
- Pick structures based on actual system needs.

# Possible additions:
AVL Tree
Red-Black Tree
Skip List
Bloom Filter
LRU Cache
Priority Queue
Suffix Array
Suffix Tree


# Bloom Filter
- Your crawler asks:
"Have I already visited this URL?"
- Instead of storing every URL lookup directly: `Bloom Filter`

- this introduces:
probabilistic data structures
false positives
memory/accuracy tradeoffs
- That's very relevant to a search engine.

# Milestone 27 — LRU Cache
- Your search engine gets repeated queries:

"python algorithms"
"python algorithms"
"python algorithms"

# Add:
LRU Cache

# Architecture:
User
 ↓
Query
 ↓
Cache ── HIT ──→ Result
 ↓ MISS
Search Engine
 ↓
Cach

# Implement the LRU yourself using:
- HashMap + Doubly Linked List

- This is an excellent DSA exercise because two structures combine to create one useful system

# Milestone 28 — RSA
- Now secure communication / document verification.

- Implement RSA educationally:
key generation
encryption
decryption
signing
verification

# You learn:
prime numbers
modular arithmetic
Euclidean algorithm
extended Euclidean algorithm
modular exponentiation


# Milestone 29 — Quantum Algorithms
- Keep this as an experimental research module rather than pretending your search engine needs quantum computing.

- Implement educational versions of:
Deutsch-Jozsa
Grover's search
Quantum Fourier Transform

# Then ask:
- What does the quantum algorithm change compared with the classical algorithm?
- That comparison is more valuable than simply implementing the circuit.



