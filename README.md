# Quadratic-Equation-Solver-in-Assembly
Project Description

This project is a Quadratic Equation Solver implemented in x86 assembly language.
The program reads the coefficients of a quadratic equation of the form: ax^2+bx+c

from the user, computes the discriminant , and determines the roots based on the value of . The program can handle all possible cases:

1: Two distinct real roots.

2: One double real root.

3: No real roots.

Additionally, the program performs error handling for invalid inputs and provides meaningful feedback to the user.

Features:

Interactive input for the coefficients.

Calculation of the discriminant ().

Detailed messaging for the nature of the roots.

Handles edge cases like:

: The equation is not quadratic.

: No real solutions.

Non-perfect square : Displays an appropriate error message.

How the Program Works

Input Handling:

The program prompts the user to input the coefficients a,b, and c using keyboard input.

A custom citireNumar procedure ensures accurate reading and conversion of numeric input.

Discriminant Calculation:

The discriminant is computed using the formula . b^2-4ac

Root Determination:

If , the program calculates two distinct roots using the quadratic formula.

If , the program calculates a single root.

If , the program displays a message stating that no real solutions exist.

Square Root Calculation:

A custom radical procedure calculates the square root of  if  is a perfect square. Otherwise, an error message is displayed.

Output:
Results are displayed to the user using the afisareNumar procedure.

Procedures Used

1. citireNumar

Reads numeric input from the user.

Handles both positive and negative numbers.

Converts ASCII characters to integers.

2. afisareNumar

Outputs a numeric value to the screen.

Handles negative numbers and zero gracefully.

3. radical

Computes the square root of a given number if it is a perfect square.

Displays an error message if the number is not a perfect square.

4. main

Coordinates the flow of the program, including input, calculations, and output.

Implements the logic for solving the quadratic equation based on the value of .

Thought Process

The program is designed to break down the solution into manageable parts, each handled by a specific procedure. This modular approach ensures clarity and reusability. The choice of assembly language highlights attention to detail and understanding of low-level programming concepts, such as:

Register manipulation

Stack operations

Conditional branching

The program is structured to anticipate and handle user errors gracefully, ensuring a robust user experience.

Example Interaction

Input:

Enter the coefficient of x^2: 1
Enter the coefficient of x: -3
Enter the constant term: 2

Output:

Delta is b^2 - 4ac: 1
x1 = 2
x2 = 1

