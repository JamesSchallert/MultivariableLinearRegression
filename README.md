# MultivariableLinearRegression
Using Numpy in Python to create a predictive model using Multivariable Linear Regression

Reads 2 columns of numbers from a text file and uses Numpy's linear algebra functions to calculate a linear regression model for
1st, 2nd, 3rd, 5th, & 7th degree polynomial functions.  This involved creating a design matrix X with (N+1) columns, where N is
the degree of the polynomial.  Each column corresponds to the value of x^n, where n is 0 to N.  You then solve for the
coefficient matrix (B) = (xTx)^-1 * (xTy), then find the predicted values of Y = XB.  I then plotted each model's predicted average
value against the raw data, as well as calculating the mean square error.  One conclusion that can be drawn from this task is that
adding more degrees of polynomials has quickly diminishing returns in reducing mean square error.  It is not shown here, but adding
more degrees of polynomials causes overfitting and reduces the model's ability to effectively predict new values, so one must be
careful when choosing number of features.  In this case, degree of the polnomial.
