# Puzzle Solver


The following program solves randomly generated minecraft puzzles and navigates the agent through the maze in the most optimal path possible. We start on the emerald block and our goal is to reach to the redstone block by traversing through the diamond blocks in between.
We first need to generate a graph containing all the possible blocks that the agent can visit. An illegal block is a "air block" in which there is no surface for the agent to stand on. Once the graph is generated, we simply assign each blocks an edge weight of 1. Dijkstra's algorithm was used specifically because it was focus of this project. It is imperative to understand the implementation here. Dijksta's algorithm basically calculates the path from the root node to every other node (i.e. block). Sometimes, this isn't what we're exactly looking for. Another approach would have been to use Uniform Cost Search. Uniform Cost Search is Dijkstra's Algorithm which is focused on finding a single shortest path to a single finishing point rather than the shortest path to every point. 

Please take a view at the implementation.
