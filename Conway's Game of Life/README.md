# Conway's Game of Life

life class methods:  
- the __init__(self, board) method takes as input an n x n numpy array of 1s and 0s, representing different cell states. A cell is considered alive if it is of state 1, and dead otherwise. The neighbors of a cell are any of the cells that are adjacent to it, 3 at a corner, 5 on an edge, 8 in the interior.  
- the run(self, n) method computes n iterations of the board and prints them  
- the plife(self) method prints the current board  
- the __next__(self) method operates on the current board, and returns the next state of the board as determined by the following rules: 

   1) If a cell is alive, and it has exactly two or three neighbors that is also alive, then in the next turn, it will remain alive.    
   2) If a cell is alive and it has less than two or more than three alive neighbors, it will die.    
   3) If a cell is dead and it has exactly three neighbors which are alive, then next turn it will come back to life. 
   4) Otherwise, it remains dead. 
