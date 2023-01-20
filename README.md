# PyTorch-Basics-and-Gradient-Descent
This is the basic of initializing Torch and their operations. It also includes gradient decent using Torch, conversion from Torch to array or array to Torch. There is also shown some codes of how to push this repository into Github. 

## Initializing Torch
Here i have shown how to intialize 1D, 2D and 3D Tensors. Tensors can have any number of dimensions, and different lengths along each dimension. We can inspect the length along each dimension using the `.shape` property of a tensor.

## Tensor operations and gradients
Here I have shown arithmetic operations, computation of derivatives, and display of the gradients.

Let `x=4`, `w=3`, `b=5` are the tensors.
`y = w * x + b`
As expected, `y` is a tensor with the value `3 * 4 + 5 = 17`. What makes PyTorch special is that we can automatically compute the derivative of `y` w.r.t. the tensors that have `requires_grad` set to `True` i.e. w and b. To compute the derivatives, we can call the `.backward` method on our result `y`. The derivates of `y` w.r.t the input tensors are stored in the `.grad` property of the respective tensors.

Here, I also show the conversion of numpy to torch and torch to numpy.
