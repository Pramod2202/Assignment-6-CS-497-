# Assignment-6-CS-497-
1. Find if Path Exists in Graph:
   Algorithm used:
     Algorithm:
      1. Create an adjacency list to represent the graph.
      2. Implement a DFS function to traverse the graph starting from the source.
      3. In the DFS function, mark visited vertices and recursively explore adjacent vertices.
      4. If the destination vertex is reached during the DFS traversal, return True.
      5. If DFS completes without reaching the destination, return False.
    Time Complexity:
      The time complexity of the DFS algorithm is O(V + E), where V is the number of vertices and E is the number of edges in the graph. In the worst case, the algorithm might visit all vertices and edges.
    Space Complexity:
      The space complexity is O(V), where V is the number of vertices. This is due to t.
