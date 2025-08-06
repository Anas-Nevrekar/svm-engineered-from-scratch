**# svm-engineered-from-scratch**
This project contains a simple and complete implementation of the Support Vector Machine (SVM) algorithm from scratch using Python, NumPy, and CVXOPT.
The SVM is trained using the dual form and solved via Quadratic Programming. The implementation supports linear, polynomial, and Gaussian (RBF) kernels, along with both hard and soft margin classification.
Features:
- No use of machine learning libraries like scikit-learn
- Supports multiple kernels (linear, polynomial, gaussian)
- Soft margin regularization using parameter C
- Dual optimization using cvxopt
- Custom bias and prediction functions

**Implementation Overview**
The SVM is implemented using the dual formulation, where the optimization problem is solved using cvxopt's QP solver. The following steps are followed in the code:

Kernel Matrix Calculation: Computes the Gram matrix using the selected kernel (linear, polynomial, or gaussian).

Quadratic Programming: Sets up and solves the dual optimization problem to find the optimal Lagrange multipliers (alphas).

Support Vector Selection:  Identifies support vectors based on non-zero alphas.

Bias Calculation: Computes the intercept b using support vectors.

Prediction: Uses the kernel function and support vectors to make predictions on new data.
