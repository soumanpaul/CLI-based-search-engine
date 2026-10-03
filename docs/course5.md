
# COURSE 5 — Approximation + Linear Programming
- This section should not be artificially forced into your basic search engine.
- nstead, introduce a new subsystem:
- `Crawler Resource Optimizer`


- Suppose your crawler has: 1,000 websites
but only: 10 workers
and: 100 GB bandwidth
- You want to maximize: information collected
- Now you have an optimization problem

# Milestone 24 — Linear Programming

- Model:

maximize:
    value_1*x1 + value_2*x2 + ...

subject to:
    cpu <= limit
    bandwidth <= limit
    workers <= limit


# Learn:
variables
objective function
constraints
feasible region
optimal solution
- Then integrate the optimizer into your crawler.


# Milestone 25 — Approximation Algorithms

- Create a problem where exact optimization is expensive.

- For example:

Select documents to crawl
such that:
    maximum coverage
    limited bandwidth


- Implement: exact algorithm
on small datasets.

- Then: approximation algorithm
on large datasets.


# Measure:
quality
runtime
memory
- Now you understand why approximation algorithms exist.

