# Graph Representations

Implement a function that converts an adjacency matrix to an adjacency list for
a directed unweighted graph using the template in `code.js`. Test your new
function; I've provided some basic testing code that uses
[jsverify](https://jsverify.github.io/) in `code.test.js`. Now, the test code
does contain the solution, so you can have a look at it if you get stuck, but
try not to peek before attempting to solve it on your own.

## Runtime Analysis

What is the runtime complexity of the conversion that you implemented? Does it
depend on the number of vertices, the number of edges, or both?

Describe your reasoning and the conclusion you've come to. Your reasoning is the
most important part. Add your answer to this markdown file.

## Answer

The runtime of this conversion is $O(|V|^2)$. We are visiting every cell in a matrix once, regardless of if it is empty or not.

We iterate over each vertex, and at each vertex, we iterate through all of its adjacent vertices. Hence our runtime complexity is $O(|V|^2)$.

It largely depends on the vertices. We will iterate through all vertices of the matrix, if we find an edge only then will we perform another operation. If we have no edges in the graph we still must check all vertices. 
## Bonus

Implement a function to convert an adjacency list to an adjacency matrix and
analyze it as above.
