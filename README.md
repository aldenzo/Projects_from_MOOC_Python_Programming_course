# Pythom_Programming_Projects-MOOC-
Below are notable projects which were completed during Python Programming Course from University of Helsinki, please find the code in src folders for each project. 

<b>1. Course_grading:</b>


- This program works with two CSV files. One of them contains information about some students on a course. The other contains the number of exercises each student has completed each week. The program asks the user for the names of these two files, reads the files, and then prints out the total number of exercises completed by each student. The exam points awarded to each student are contained in a CSV file. The program should again ask the user for the names of the files. Then the program should process the files and print out a grade for each student.

- Each completed exercise is counted towards exercise points, so that completing at least 10 % of the total exercices awards 1 point, completing at least 20 % awards 2 points, etc. Completing all 40 exercises awards 10 points. The final grade for the course is determined based on the sum of exam and exercise points. For (exam points + exercise points) and equivalent grades: 0-14 :	0 (fail) | 15-17	: 1 | 18-20	: 2 | 21-23	: 3 | 24-27	: 4 | 28-	: 5 |

- We now shall print out some statistics based on the CSV files. Each row contains the information for a single student. The number of exercises completed, the number of exercise points awarded, the number of exam points awarded, the total number of points awarded, and the grade are all displayed in tidy columns. The width of the column for the name should be 30 characters, while the other columns should be 10 characters wide.

- We'll add a file containing information about the course. The program should then create two files. There should be a file called results.txt. The statistics section is identical to the results printed out in part 3 of the project. The only addition here is the header section. Additionally, there should be a file called results.csv. That is, the program only asks for the names of the input files. All output should be written to the files. The user will only see a message confirming this.

The above is the sample desired output: 
<h3><img height="500" src="%20Images/course_grading_output.png"></h3>



<b>2. Letter_square:</b>

The program which prints out a square of letters with the numbers of layers as the input. The output can be specified in the examples below. We may assume there will be at most 26 layers.

<h3><img align="left" height="300" src="%20Images/letter_square3.png"> <img align="center" src="%20Images/letter_square4.png" height="300"></h3>



<b>3. Sudoku_game:</b>

<b>3.1 Sudoku_play:</b>

The function print_sudoku(sudoku: list) takes a two-dimensional array representing a sudoku grid as its argument. The function should print out the grid in the specified format. The function add_number(sudoku: list, row_no: int, column_no: int, number:int) takes a two-dimensional array representing a sudoku grid, two integers referring to the row and column indexes of a single square, and a single digit between 1 and 9, as its arguments. The function should add the digit to the specified location in the grid.


<b>3.2 Sudoku_check:</b>

Create 2 functions named row_correct(sudoku: list, row_no: int) and column_correct(sudoku: list, column_no: int), which takes a two-dimensional array representing a sudoku grid, and an integer referring to a single row/column, as its arguments. Rows and columns are indexed from 0. The function should return True or False, depending on whether the row / column is filled in correctly, that is, whether it contains each of the numbers 1 to 9 at most once.

Create function named block_correct(sudoku: list, row_no: int, column_no: int), which takes a two-dimensional array representing a sudoku grid, and two integers referring to the row and column indexes of a single square, as its arguments. Rows and columns are indexed from 0. The function should return True or False depending on whether the 3 by 3 block to the right and down from the given indexes is filled in correctly. That is, whether the block contains each of the numbers 1 to 9 at most once.

Complete function named sudoku_grid_correct(sudoku: list), which takes a two-dimensional array representing a sudoku grid as its argument. The function should use the three previous functions to determine whether the complete sudoku grid is filled in correctly. The function should check each of the nine rows, columns and 3 by 3 blocks in the grid. If all contain each of the numbers 1 to 9 at most once, the function returns True. If a single one is filled in incorrectly, the function returns False. The image of a sudoku grid has the nine blocks within the grid indicated with thicker borders. These are the blocks the function should check, and they begin at the indexes (0, 0), (0, 3), (0, 6), (3, 0), (3, 3), (3, 6), (6, 0), (6, 3) and (6, 6).

<h3><img align="left" height="500" src="%20Images/sudoku_play_sample.png"> <img align="center" src="%20Images/sudoku_play_output.png" height="500"></h3>


