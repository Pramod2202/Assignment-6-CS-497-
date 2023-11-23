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
          The space complexity is O(n) due to the `visited` array used to store the state of each node during the DFS traversal. The depth of the recursion stack is also proportional to the number of nodes in the worst case.

3. Connecting cities with minimum cost:
     Algorithm:
          1. Sort the connections by their costs in ascending order.
          2. Initialize a disjoint set data structure using the `find` and `union` functions.
          3. Iterate through the sorted connections and add the edge to the spanning tree if it doesn't create a cycle.
          4. Keep track of the total cost and the number of edges added.
          5. If the number of edges added is equal to N - 1 (the number of cities minus one), return the total cost; otherwise, return -1.
   Time Complexity:
     The time complexity is O(E * log(E)) where E is the number of connections. The dominant factor is the sorting of connections.
   Space Complexity:
     The space complexity is O(N) for the parent and rank arrays.

4. All paths from source to Target:
     Algorithm:
             Implement a DFS function (dfs) that takes the current node and the current path as parameters.
             If the current node is the destination (node n-1), add a copy of the current path to the result.
             Recursively explore all neighbors of the current node by calling dfs for each neighbor.
             Start DFS from the source node (node 0) with an initial path containing only the source node.
     Time Complexity:
          The time complexity is O(2^N), where N is the number of nodes. In the worst case, all possible paths are explored.

     Space Complexity:
          The space complexity is O(N), where N is the number of nodes. This includes the space required for the recursive call stack during DFS.


