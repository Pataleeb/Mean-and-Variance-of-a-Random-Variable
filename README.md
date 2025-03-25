# Mean-and-Variance-of-a-Random-Variable
Estimating Mean and Variance Functions of a Random Variable Dependent on Two Independent Variables

Overview: In probability and statistics, it is important to understand the mean and variance for any random variables. In many applications, it is straightforward to simulate the random variable Y ’s, but it is often highly non-trivial to characterize the exact distribution of Y = Y (X1, X2) including deriving the explicit formulas for the mean and variance of Y = Y (X1, X2) explicitly as a function of X1 and X2.

Objective: Suppose that Y = Y (X1, X2) is a random variable whose distribution depends on two independent variables X1 and X2, and the objective is to estimate two deterministic functions of X1 and X2: one is the mean µ(X1, X2) = E(Y ) and the other is the variance V (X1, X2) = Var (Y ).
For that purpose, we are provided the observed 200 realizations of the Y ’s values for some given pairs (X1, X2)’s. We are asked to use data mining or machine learning methods that allow us to conveniently predict or approximate the mean and variance of Y = Y (X1, X2) as a function of X1 and X2. That is, our task is to predict or approximate two values for those given pairs (X1, X2) in the testing data set: one for the mean µ(X1, X2) = E(Y (X1, X2)) and the other for the variance V (X1, X2) = V ar(Y (X1, X2)).

Training data set: In order to develop a reasonable estimation of the mean and variance of Y = Y (X1, X2) as deterministic functions of X1 and X2, we provide a training data set that is generated as follows. We first choose the uniform design points when 0 ≤ X1 ≤ 1 and 0 ≤ X2 ≤ 1, that is, x1i = 0.01 ∗ i for i = 0, 1, 2, . . . , 99, and x2j = 0.01 ∗ j for j = 0, 1, 2, . . . , 99. Thus there are a total of 100 ∗ 100 = 104 combinations of (x1i, x2j)’s, and for each of these 104 combinations, we generate 200 independent realizations of the Y variables, denoted by Yijk for k = 1, . . . , 200.

Note that this training data set is a 104 ×202 table. Each row corresponds to one of 100∗100 = 104 combinations of (X1, X2)’s. The first and second columns are the X1 and X2 values, respectively, whereas the remaining 200 columns are the corresponding 200 independent realizations of Y ’s.

Based on the training data, we are asked to develop an accurate estimation of the functions µ(X1, X2) = E(Y ) and V (X1, X2) = Var (Y ), as deterministic functions of X1 and X2 when 0 ≤ X1 ≤ 1 and 0 ≤ X2 ≤ 1.

Testing data set: For the purpose of evaluating our proposed estimation models and methods, we choose 50 random design points for X1 and 50 random design points for X2. Thus there are a total of 50 ∗ 50 = 2500 combinations of (X1, X2) in the testing data set. We are asked to use our formula to predict µ(X1, X2) = E(Y ) and V (X1, X2) = Var (Y ) for Y = Y (X1, X2) for the 50 ∗ 50 = 2500 combination of (X1, X2) in the testing data.


