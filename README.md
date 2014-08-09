#Union Find

A union-find algorithm is an algorithm that performs two useful operations on such a data structure:

* Find: Determine which subset a particular element is in. This can be used for determining if two elements are in the same subset.
* Union: Join two subsets into a single subset.


To make both union and find efficient, we have to implement two enhancements.

##Union by Rank
Always attach the smaller tree to the root of the larger tree.

##Path compression
As _find_ recursively traverses up the tree, change each node's parent reference to point to the root that it had found. The resulting tree is much flatter.

