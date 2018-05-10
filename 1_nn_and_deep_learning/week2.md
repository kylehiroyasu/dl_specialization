### Week 2 Neural Network Basics:

#### Binary Classification

Models which have 0 or 1 output.
With these kinds of models, such as logistic regression, we need some labeled data with the format:
*{x_1, y_1},...{x_m, y_m}*

We also want to split the data into training and testing groups

A useful notation for implementing NN is to use the training examples as matrices where each observation *x_i* and *y_i* are basically column vectors.

#### Logistic Regression

A binary classification algorithm. Can be used to predict a true/false or group1/group2 outcome.

Given some *x* want to predict *y_hat = P( y = 1 | x)* where *x* is an element of some vectorspace *R_n_x*
using parameters *w* which is an element of *R_n_x* and *b* element of *R_1*

Typically we use the sigmoid function for logistic regression:

* sigma(z) = 1 / (1 + e^-z) *

#### Logistic Regression Cost Funtion

A Loss function should be able to tell us how well our and ideally will be convex in shape. This is very useful when training our model/optimizing parameters because it allows us to find a global minimum instead of a local minimum.

For logistic regression we will use the following loss function:
*L(y, y_hat) =  - (y log(y_hat) + (1-y) log(1-y_hat)) *

and we will average over our *m* training examples to obtain our cost function:
* J(w,b) = (1/m) \* sum(L(y, y_hat)) *

Logistic regression can also be represented as a very small NN.

#### Gradient Descent

Gradient descent is a method of training an algorithm to iteratively minimize the cost function and optimize algorith performance.

Typically with Logistic Regression the parameters *w* and *b* are initialized to 0.

Using our learning rate *alpha* we subtract *alpha \* dJ(w)/ dw* to slowly change *w* until we acheive a global minimum.

#### Derivatives

Skipped


#### More Derivative Examples

Skipped

#### Computation Graph

Compute left to right?

#### Derivatives with a Computation Graph

Don't forget to use the chain rule to decompose the derivative of complex functions

*dvar* represents the derivative of the final output (for example cost function) with respect to the various intermediate variables.


#### Logistic Regression Gradient Descent

*a-y*

#### Gradient Descent on m Examples

Instead of taking the partial derivatives for a single training example our convex cost function is the average of the loss function over all of our training examples.