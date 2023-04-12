# Sudoku-Solver
Sudoku Solver using Computer Vision and Image Processing
This project is a Sudoku Solver that uses Computer Vision and Image Processing techniques to read and solve a 9x9 grid Sudoku puzzle. The solver is written in Python and uses the OpenCV library for image processing and NumPy for array manipulation.


### Installation and Usage:

To use this Sudoku Solver, you will need to have Python 3.x installed on your system along with the OpenCV and NumPy libraries. You can install them using pip by running the following commands:


pip install opencv-python

pip install numpy

To run the solver, simply clone this repository and run the sudoku_solver.py file. Make sure to place an image of the Sudoku puzzle in the input folder before running the solver. The solved Sudoku puzzle will be displayed on the screen.

### How it works:

The Sudoku Solver works by first reading the image of the Sudoku puzzle using the OpenCV library. The image is then preprocessed to enhance the contrast and remove any noise or unwanted elements.

Next, the grid lines of the Sudoku puzzle are detected using Hough Transform. Once the grid lines are detected, the cells of the Sudoku puzzle are extracted and processed individually.

For each cell, the digit is extracted by first thresholding the cell and then finding the contour with the largest area. The digit is then recognized using a machine learning model trained on the MNIST dataset.

Once all the digits are extracted and recognized, the solver uses a backtracking algorithm to solve the Sudoku puzzle. The algorithm checks if the current digit is valid and if it is, moves on to the next cell. If the current digit is not valid, the algorithm backtracks to the previous cell and tries a different digit.

### Conclusion:

In conclusion, this Sudoku Solver uses Computer Vision and Image Processing techniques to read and solve a 9x9 grid Sudoku puzzle. It is a fun project to work on and can be extended to solve more complex Sudoku puzzles. If you have any questions or suggestions, please feel free to contact me.
