# Topic: Logsitic Regression

**Author**: Anusiem John-Franklin

**QAs Total:** 3

The following are questions accompanied with their answers found on the internet on Logistic Regression. The level of difficulty is divided into 3:

1. Junior 
2. Medium 
3. Senior

---

## Q : Why can’t we use Mean Square Error (MSE) as a cost function for logistic regression?

**Difficulty:** `Junior`

**Source:** 


**Answer:**
In logistic regression, we use the sigmoid function and perform a non-linear transformation to obtain the probabilities. Squaring this non-linear transformation will lead to non-convexity with local minimums. Finding the global minimum in such cases using gradient descent is not possible. Due to this reason, MSE is not suitable for logistic regression. Cross-entropy or log loss is used as a cost function for logistic regression. In the cost function for logistic regression, the confident wrong predictions are penalised heavily. The confident right predictions are rewarded less. By optimising this cost function, convergence is achieved.

---

## Q : How does logistic regression handle categorical variables?

**Difficulty:** `Mid`

**Source:** 


**Answer:**
The inputs to a logistic regression model need to be numeric. The algorithm cannot handle categorical variables directly. So, they need to be converted into a format that is suitable for the algorithm to process. 
The various levels of a categorical variable will be assigned a unique numeric value known as the dummy variable. These dummy variables are handled by the logistic regression model as any other numeric value. So of the approaches used are:
1. Using the LabelBinarizer from sklearn
2. Using BinaryEncoder from category_encoders
3. Using the get_dummies() function of the pandas library

---

