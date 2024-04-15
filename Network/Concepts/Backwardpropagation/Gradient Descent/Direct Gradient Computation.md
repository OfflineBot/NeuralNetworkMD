# Direct Gradient Computation

$W\_input = dot(norm\_input^T, loss * deriv(z1))$
$W\_hidden = dot(a1^T, loss * deriv(z2))$
$B\_hidden = sum(W\_input, axis=0)$
$B\_output  = sum(W\_hidden, axis=0)$

Where:
- $W\_input$: the Gradient of the weight from input-hidden
- $W\_hidden$: the Gradient of the weight from hidden-output
- $B\_hidden$: the Gradient of the bias from the hidden
- $B\_output: the Gradient of the bias from the output$
- $norm\_input^T$: Transposed input
- $a1^T$: Transposed activated output of first linear calculation
- $deriv(z1)/deriv(z2)$: derivative activation function from [[Forward Propagation|Forwarded]] output
- $loss$: the loss from output, target