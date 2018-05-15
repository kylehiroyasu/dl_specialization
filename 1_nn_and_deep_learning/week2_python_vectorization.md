### Python and Vectorization

#### Vectorization

The ability to use vectorized code instead of `for-loops` is critical for performant machine learning code. 

Whenever possible avoid explicit for loops

#### More Vectorization Examples

Nothing new

#### Vectorizing Logistic Regression

When you add a real number to a vector in python it is called 'broadcasting'

#### Vectorizing Logistics Regression's Gradient Output

He provides a vectorized version of gradient descent back propogation

#### Broadcasting in Python

Broadcasting is helpful for optimizing python code

#### A note on python/numpy vectors

Broadcasting can introduce subtle and confusing bugs.

Rank one arrays in particular can be tricky because they don't behave consistently like matrices/vectors

don't use:
`np.random.randn(3)`

use:
`np.random.randn(3,1)`

Then the datastructure will behave normally and intuitively
also use statements like `assert(a.size == [3,5])` to guarantee your datastructures are as expected.

#### Tour of Jupyter notebooks

Just using jupyter notebooks

#### Explanation of logistic regression cost function

