Go Rope Data Structure
======================

Immutable, cache optimized, thread safe data structure for storing string data.
Especially ones on the larger side that are execting frequent inserts, removes, substrings/clone operations.

Strictly speaking, the actual 'string' data is stored in slab-alocated 4kb byte arrays, and the the 'tree' nodes
simiply slab-alocated and similaly actaully jammed into 4kb byte arrays.

The intend here is to maximize cache locality and minimize memory fragmentation,while still providing technically
modelling an immutable tree data structure.
