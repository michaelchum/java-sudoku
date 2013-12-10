java-sudoku
===========

A sudoku solver for 3x3, 4x4 and 5x5 boards aimed for speed

Can solve 3x3 grids in under 30ms

4x4 and 5x5 grids between 150ms to 40s depending on difficulty (empty slots and positioning)

Speed improvements to come

Input format of the sudoku grid is as follows in .txt file

``
3

x x x | x x x | x x x
x 1 x | 6 2 x | x 9 x
x x 2 | x x 9 | 3 1 x
---------------------
x x 4 | x x 6 | x 8 x
x x 8 | 7 x 2 | 1 x x
x 3 x | 8 x x | 5 x x
---------------------
x 6 9 | 1 x x | 4 x x
x 8 x | x 7 3 | x 5 x
x x x | x x x | x x x

(Evil puzzle from www.websudoku.com)
``
``
5

 1  4 23  x 12 |  3  x  x 14 11 |  x 17 25  x 22 |  x 16  9 13 20 |  x  x  x  x 24 
10  x  x  3  x |  9  x 15  2  x | 21  x 11  x  5 |  x  8  1 25  x |  x  7  x  x 14 
 x 11 22  8  x |  x 19  x 12 17 | 13  x  2  x  x | 23 14  3  x  x |  x  x  x  x  5 
20  x  x 16  7 |  x  x 25 13  1 |  x 14 19 24  x |  5  x  x  x  x |  x  x  8  x  x 
 x 25  5 13  2 |  x  6 21 16  x |  9 23  x  x  x |  x  x  x  x 17 |  x 12 11  x 10 
----------------------------------------------------------------------------------
 9  6 21  x  x | 19  7  x  x 22 |  4  3  8 13  x |  2  x  x 24 23 | 16  1  x 14  x 
 7  x  x 23  x |  x  1  x  x 14 |  x 21  x  6 16 | 12 19  x 15 10 |  x  4  x 13 11 
 x  x  x  x  x |  5 17  9 10 24 | 23  x  x  x 14 | 25  x  x 21  8 |  2  x 15  x  x 
 x  x  x  x  x |  x 16  x  4 25 | 10 11  x  x  x |  x  3 14  x  x |  x 23  x 19  7 
 x 13  x  x 19 | 15  x 11 23  x | 22 20  x 18  x |  x  x  7  x  x |  6  x 10 24  8 
----------------------------------------------------------------------------------
 x  8  x  x  x |  x  x  x  9  3 |  x 12  x 23  x |  x  1 22  x  x |  x  x  x  5  x 
24  2 11  x  x | 12 25 17  x  x |  x  7  x  4  x |  x  x 15  8  x |  x  x  x  x 16 
19 21 12  x  x |  x  x  x  x  x |  x  x 18  x  x |  x  x  x  x  x |  x  x 13  9  4 
 6  x  x  x  x |  x 22 14  x  x |  x 15  x 25  x |  x  x 23 17  4 |  x  x 18 12 21 
 x 18  x  x  x |  x  x  1  6  x |  x 22  x  5  x |  7 21  x  x  x |  x  x  x 25  x 
----------------------------------------------------------------------------------
15 17  9  x 13 |  x  x  4  x  x |  x 16  x 11 23 |  x 24 12  x  3 | 22  x  x  8  x 
16  7  x  6  x |  x  x 12 11  x |  x  x  x  3 19 | 17  2  x  4  x |  x  x  x  x  x 
 x  x  x  x  4 | 17  3  x  x  2 | 12  x  x  x 24 |  9  6 20 18  1 |  x  x  x  x  x 
11  3  x 19  x | 14 23  x 24  9 |  6 25  x 20  x | 13  x  x  5  x |  x 16  x  x 18 
 x 12  x 18 24 |  6 13  x  x 20 |  x  9 21 17 15 |  8  x  x 23 11 |  x  x  3  4  2 
----------------------------------------------------------------------------------
 2  x 16  4  x |  1  x  x  x  x |  x  x  x 21  8 |  x  7  5 22  x | 24 13 12 10  x 
 x  x 24  x  x |  x  x  x  x 21 |  x  4 12  1  x | 16 20 10  x  x | 18 25  x  x 23 
18  x  x  x  x |  x  x  8 19 10 |  x  x  6  x  7 | 15 17  x  1  x |  x  2 14 20  x 
13  x  x  1  x |  x  4 18 15  x |  5  x 24  x 17 |  x 23 19  x 14 |  x  6  x  x  3 
22  x  x  x  x | 23 12 24 17  x | 16  x 14 10  x |  6 25  x  x 21 |  4  x  9 15  1 

(5x5 Sudoku puzzle from www.menneske.no/sudoku/5/eng/)
``