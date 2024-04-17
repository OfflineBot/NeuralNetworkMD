# Matrix Multiplication
A way to multiply Matrices together.
To make it work the columns of the first Matrix and the rows of the second Matrix must match.

## Example:
$\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} * \begin{bmatrix} 1 & 2 \\ 3 & 4 \\ 5 & 6 \end{bmatrix} = \begin{bmatrix} (1 * 1 + 2 * 3 + 3 * 5) & (1 * 2 + 2 * 4 + 3 * 6) \\ (4 * 1 + 5 * 3 + 6 * 5) & (4 * 2 + 5 * 4 + 6 * 6) \end{bmatrix} = \begin{bmatrix} 22 & 28 \\ 49 & 64 \end{bmatrix}$

$\begin{bmatrix} 1 & 2 \\ 3 & 4 \\ 5 & 6 \end{bmatrix} * \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} = \begin{bmatrix} (1 * 1 + 2 * 4) & (1 * 2 + 2 * 5) & (1 * 3 + 2 * 6) \\ (3 * 1 + 4 * 4) & (3 * 2 + 4 * 5) & (3 * 3 + 4 * 6) \\ (5 * 1 + 6 * 4) & (5 * 2 + 6 * 5) & (5 * 3 + 6 * 6) \end{bmatrix} = \begin{bmatrix} 9 & 12 & 15 \\ 19 & 26 & 33 \\ 29 & 40 & 51 \end{bmatrix}$
