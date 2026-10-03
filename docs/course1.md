# COURSE 1 CHECKPOINT
Array
String algorithms
Hash table
Linked list
Stack
Queue
Heap
Searching
Sorting
Complexity analysis

# Search Engine v1

Documents
    ↓
Tokenizer
    ↓
Inverted Index
    ↓
Search
    ↓
Heap
    ↓
Top-K Results


# COURSE 1 — Foundations

# Milestone 1 — `Document Store`
- `Product requirement`: Your system needs to store documents.
# A document:
{
  "id": 123,
  "title": "Introduction to Algorithms",
  "content": "...",
  "url": "...",
  "created_at": "..."
}
- Start with 100–1,000 documents.
- Don't use Elasticsearch.
- Don't use a database for search.
- Build the search machinery yourself.


# DSA: Arrays: Implement
- DynamicArray
# Support:
append()
insert()
delete()
get()
set()
resize()

- Then ask: What is the complexity of each operation?
- Create a benchmark.
N = 10
N = 100
N = 1,000
N = 10,000
N = 100,000
# Record:
operation
N
time
memory


# Milestone 2 — Text Processing
- Now your product needs to understand text.

# Implement:
tokenize()
normalize()
lowercase()
remove_punctuation()
remove_stop_words()

Example: "Algorithms, Data Structures & Graphs!"
becomes: ["algorithm", "data", "structure", "graph"]

# You can then learn:
strings
arrays
hashing
sorting

# Milestone 3 — Hash Table
- Now you discover a product problem: "Given a word, which documents contain it?"

- You need: word → documents
- Implement your own: HashTable
- Then: InvertedIndex


# Conceptually:
"algorithm"
    ↓
[doc1, doc7, doc23, doc91]

"graph"
    ↓
[doc2, doc7, doc32]
- This becomes the foundation of your search engine.
# DSA learned
- Hash table
- collision handling
- load factor
- resizing
- average vs worst-case complexity


# Milestone 4 — Searching
- Implement:
    - linear_search()
    - binary_search()
- Then apply binary search to sorted document IDs / posting lists.
- You'll discover something important: The algorithm is only useful if the underlying data is structured appropriately.
- That is a major DSA lesson.

# Milestone 5 — Sorting
- Implement yourself:
bubble_sort
insertion_sort
selection_sort
merge_sort
quick_sort
heap_sort

# Build a benchmark:
Algorithm       1K      10K      100K
----------------------------------------
Insertion
Merge
Quick
Heap
- Then use sorting inside your search engine

# For example:
results
   ↓
sort by relevance
   ↓
top 10

# Milestone 6 — Stack + Queue
- Now build the crawler.
- You have URLs:
page A
 ↓
page B
 ↓
page C
 ↓
page D

- A crawler needs a frontier
- Queue<URL>

- Implement: Queue
- Then use it for: BFS crawler
- A stack can be used for: DFS crawler
- Now you have an actual reason to understand: BFS vs DFS
rather than memorizing it.

# Milestone 7 — Linked List
- Build:
LinkedList
DoublyLinkedList

- Then use it in your hash table:
Hash bucket
     ↓
Linked List

- This gives you a real reason to understand collision resolution.

# Milestone 8 — Heap
- Now search becomes: "Return the top 10 most relevant documents."
- You don't need to fully sort 1 million documents.

- Use: MinHeap
- Keep only: Top K documents.

- This introduces: O(N log K)
- instead of potentially: O(N log N)
- This is exactly the kind of thinking I want you to develop.



# Prompts
- If you want to do this seriously, the next step should be Milestone 1, where we design the actual project requirements, database/schema, folder structure, CLI commands, test strategy, and your first DynamicArray implementation before writing the search engine itself.