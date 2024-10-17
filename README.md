Gaussian Elimination Solver

Overview:

This is a C# application that implements Gaussian elimination to solve systems of linear equations. It is designed with a simple graphical user interface (GUI) to allow users to input the coefficients of three linear equations in three variables. The application performs Gaussian elimination and outputs the values of the unknowns, if a solution exists.

Language:

The program is written in C# using Windows Forms for the graphical user interface (GUI).

How it Works:

User Input:

The GUI consists of text boxes where the user inputs the coefficients for a system of three linear equations.
There are labels and buttons to guide the user in providing valid input.

Validation:

The program validates the input to ensure there are no empty fields or invalid coefficients. It also checks for impossible configurations, such as an equation like 0x1 + 0x2 + 0x3 = 1.

Gaussian Elimination:

The core of the application lies in the logic that applies Gaussian elimination to solve the system of equations.
The method involves transforming the system into an upper triangular form and then using back-substitution to find the values of the unknowns.

Steps in Gaussian Elimination:

The program normalizes the first equation by dividing all terms by the coefficient of x1.
It then eliminates x1 from the subsequent equations by adjusting them with the first equation.
This process is repeated for x2 and x3, after which the values of the unknowns (x1, x2, x3) are calculated.
The solution is printed in the GUI.

Output:

The calculated values for x1, x2, and x3 are displayed in a read-only text area.
The program also checks if the system has no solution or infinitely many solutions and informs the user accordingly.

Reset Functionality:

The user can reset the input fields to start over by pressing the "Reset" button.

Features:

Input Validation: Ensures the system of equations entered is valid and solvable.
Solution Output: Displays the solution or an error if the system is inconsistent or has infinite solutions.
User-Friendly GUI: Simple, interactive interface for easy input of equations.

Usage:

Enter the coefficients for three equations in the provided text boxes.
Click the "Aprēķināt" (Calculate) button to solve the system.
The solution will be displayed, or an error message will appear if the system is unsolvable.
To reset, click the "Atiestatīt" (Reset) button.

Requirements:

.NET Framework
Windows operating system
