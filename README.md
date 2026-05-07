# QuasiNewton_BFGS-APP-
A Maple Maplet GUI for fixed-step BFGS Quasi-Newton optimization with user-defined function, variables, initial point, alpha, tolerance, and detailed iteration-by-iteration numerical output.


# Fixed-Step BFGS Quasi-Newton Solver in Maple

This project implements a graphical Maple Maplet application for solving unconstrained nonlinear optimization problems using the BFGS Quasi-Newton method.

The solver uses the update rule:

x_{k+1} = x_k + alpha_k p_k

where the search direction is obtained from:

B_k p_k = -grad f_k

The initial matrix B_0 is set to the identity matrix, and the step length alpha_k can be entered by the user through the GUI.

## Features

- Maple Maplet graphical user interface
- User-defined objective function
- User-defined variables and initial point
- Adjustable step length alpha_k
- Adjustable tolerance and maximum iterations
- Automatic symbolic gradient calculation
- Automatic symbolic Hessian calculation
- BFGS matrix update
- Detailed iteration-by-iteration output
- Superlinear condition value calculation:

||grad f_k + Hessian f_k p_k|| / ||p_k||

## Example

Objective function:

f(x) = x1^2 + 2*x2^2

Variables:

[x1, x2]

Initial point:

[2, 1]

The program displays all intermediate values, including x_k, f_k, grad f_k, B_k, p_k, s_k, y_k, B_{k+1}, and the final result.
