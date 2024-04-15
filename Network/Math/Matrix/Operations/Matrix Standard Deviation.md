# Matrix Standard Deviation
Calculate the standard deviation for Matrices.

## Steps:
- Subtract the mean of the Matrix
- Square the result
- Take the mean of that
- Take the square root of the result
For Axis 0 take every mean at Axis 0.
For Axis 1 take every mean at Axis 1.

## Example:
Starting Matrix: $\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix}$

For Axis 0:
- Subtract the mean (Axis 0)
$\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} - \begin{bmatrix} 2.5 & 3.5 & 4.5 \end{bmatrix} = \begin{bmatrix} -1.5 & -1.5 & -1.5 \\ 1.5 & 1.5 & 1.5 \end{bmatrix}$
- Square the result
$\begin{bmatrix} -1.5^2 & -1.5^2 & -1.5^2 \\ 1.5^2 & 1.5^2 & 1.5^2 \end{bmatrix} = \begin{bmatrix} 2.25 & 2.25 & 2.25 \\ 2.25 & 2.25 & 2.25 \end{bmatrix}$
- Take the mean (Axis 0)
$\begin{bmatrix} 2.25 & 2.25 & 2.25 \\ 2.25 & 2.25 & 2.25 \end{bmatrix} \textrightarrow \begin{bmatrix} 2.25 & 2.25 & 2.25 \end{bmatrix}$

- Take the square root of each element
Result: $\begin{bmatrix} 1.5 & 1.5 & 1.5 \end{bmatrix}$
