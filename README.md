# BFS-Image-Maze-Solver 
A project to implement the BFS algorithm to create a maze image solving program.

Intended Outcome: 
  -To be able to take in an image, of certain color and format constraints, and return a copy of that image with the shortest path from the beginning pixel (red) to the end pixel (blue)

Intended Process: 
  -Read in the maze image using Image module from PIL 
  -Convert image into a 2D array of int values based on the color of each pixel 
  -Use the BFS algorithm to find shortest, starting from start pixel, tot the goal pixel 
  -When the BFS algorithm reaches the goal pixel, retrace the steps and send back the path 
  -Apply the path to the 2D grid and convert the grid back into an image
