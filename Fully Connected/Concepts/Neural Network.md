# Neural Network
Layout of the Neural Network:

### Layout:
1. Getting Data
	- Input Data
	- Corresponding Output
	- New Data
2. [[Normalization|Normalize]] the Data
	- Only Input Data
3. [[Initialization|Initialize]] the Parameters
	- [[Hyperparameter]]
	- Weights
	- Biases
4. Define the [[Loss]]- and [[Activation Function|Activation]] Function
5. [[Training|Train]] the Dataset
	- [[Forward Propagation]]
	- [[Backward Propagation]]
	- [[Optimization]]
1. [[Validation|Validate]] the Results

### Example:
Not a real code. Just a **Pseudo Code** orientated at Python.
```py
# Task: Bit wise OR
input_data = [[1, 1], [0, 0], [1, 0], [0, 1]]
truth_data = [[0], [0], [1], [1]]
new_input_data = [[1, 1], [0, 0], [1, 0], [0, 1]] # For other examples this would change

# Normalize it (Data is small so no need here)

# Hyperparameter
iterations = 100
learning_rate = 0.01
input_size = input_data[0].size() # 2
hidden_size = 10
output_size = output_data[0].size() # 1

# Initialize Weights and Biases randomly
# Weights:
w1 = array_size(input_data, hidden_data).random_uniform(-1.0, 1.0)
w2 = array_size(hidden_data, output_data).random_uniform(-1.0, 1.0)
# Biases:
b1 = array_size(hidden_data).random_uniform(-1.0, 1.0)
b2 = array_size(output_data).random_uniform(-1.0, 1.0)

# Loss
def loss(output, truth) ...
# Activation
def activation(x) ...
def deriv_activation(x) ...

# Training
for x in range(iterations):

	# Forward Propagation
	output = forward(input_data)
	
	loss = loss(output, truth_data)
	# handling loss	
	if (i % 100 == 0):
		print(f"Loss: {loss} | Iteration: {x}")

	# Backward Propagation
	# Calculate Gradients (HERE Direct Gradient Computation)
	w1_grad, w2_grad = ...
	b1_grad, b2_grad = ...
	# Apply Optimization Algorithm (HERE SGD)
	w1 -= learning_rate * w1_grad
	w2 -= learning_rate * w2_grad
	b1 -= learning_rate * b1_grad
	b2 -= learning_rate * b2_grad

# Validation
output = forward(new_input_data)
print(output)
```