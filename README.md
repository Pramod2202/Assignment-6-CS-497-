# Assignment-6-CS-497-
1. Find if Path Exists in Graph:
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

2. Longest cycle in a Graph:
      Algorithm:
          1. DFS Traversal:
             - The algorithm uses Depth-First Search (DFS) to traverse the graph.
             - It maintains a `visited` array to keep track of the state of each node during the DFS traversal.
             - When a node is visited with a value of 1, it indicates that a cycle is found, and the length of the cycle can be calculated.
             - If a node is visited with a value of 2, it means the node is part of a previously explored path and does not contribute to the cycle.
          2. Cycle Length calculation: The `dfs` function is recursively called to explore the graph and calculate the length of cycles.
          3. Main Loop: The main loop iterates through each node in the graph and initiates DFS if the node hasn't been visited.
          4. Result: The maximum cycle length is tracked, and the result is returned.
      Time Complexity:
          The time complexity is O(n), where n is the number of nodes in the graph. Each node is visited at most once during the DFS traversal.
      Space Complexity:
          The space complexity is O(n) due to the `visited` array used to store the state of each node during the DFS traversal. The depth of the recursion stack is also proportional to the number             of nodes in the worst case.


