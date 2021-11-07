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
  
How to Use:
  -Clone repository
  
  -Input path from current directory to test maze image desired in BreadthFirstSearchImage.py in main function
    EX: img = Image.open("/TestMazes/TestMaze1.png")
 
  -Execute BreadthFirstSearchImage.py
  
Instruction to Create Own Maze  (capitalized colors have specific RGB/RGBA values):

  -Access image creating program/website with pixel specific editing tools
    EX: https://www.pixilart.com/
    
  -Setup initial maze with a BLACK outer border and WHITE inner area
    EX: See TestMaze 1-4
  
  -Add a single RED pixel to act as start
    EX: See TestMaze 1-4
  
  -Add a single BLUE pixel to act as goal
    EX: See TestMaze 1-4
  
  -Add any obstacles or path restrictions with BLACK pixels
    EX: See TestMaze 1-4
  
  -Save image as PNG
  
  Color Specifications (RGB/RGBA):
  
    -BLACK: (0,0,0) / (0,0,0,255)
    
    -WHITE: (255,255,255) / (255,255,255,255)
    
    -RED: (233,30,99) / (233,30,99,255)
    
    -BLUE (63,81,181) / (63,81,181,255)
    
  -WARNING: Personal computers/image creation software may interpret/save colors differently and raise an Unrecognized Color Value Exception. To fix, edit the ImageHandle.py file's pixToSym function. The conditional of that function checks for a BLACK, WHITE, RED, and BLUE color in that order. Change the corresponding tuple of the intended color to the color tuple given in the exception.

