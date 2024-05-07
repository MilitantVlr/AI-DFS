# AI-DFS
# Ex.No: 2  Implementation of Depth First Search
### DATE: 17/02/2024                                                                           
### REGISTER NUMBER : 212221040145
### AIM: 
To write a python program to implement Depth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function dfs and take the set “visited” is empty 
4. Search start with initial node. Check the node is not visited then print the node.
5. For each neighbor node, recursively invoke the dfs search.
6. Call the dfs function by passing arguments visited, graph and starting node.
7. Stop the program.
### Program:
```python
graph = {
    '5': ['3', '7'],
    '3': ['2', '4'],
    '7': ['8'],
    '2': [],
    '4': ['8'],
    '8': []
}
visited = set()
def dfs(graph, node):
    if node not in visited:
        print(node)
        visited.add(node)
        for neighbour in graph[node]:
            dfs(graph, neighbour)
print("Following is the Depth-First Search:")
dfs(graph, '5')
```
### Output:
![DFS](https://github.com/MilitantVlr/AI-DFS/assets/121683193/01b2fbb6-7d20-4cd4-95ae-5379e5a5fc37)

### Result:
Thus the depth first search order was found sucessfully.
