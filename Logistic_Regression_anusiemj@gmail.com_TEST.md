# Topic: Logsitic Regression

**Author**: Anusiem John-Franklin

**QAs Total:** 3

The following are questions accompanied with their answers found on the internet on Logistic Regression. The level of difficulty is divided into 3:

1. Junior 
2. Medium 
3. Senior

---

## Q1 : How does logistic regression handle categorical variables?

**Difficulty:** `Junior`

**Source:** 


**Answer:**
The inputs to a logistic regression model need to be numeric. The algorithm cannot handle categorical variables directly. So, they need to be converted into a format that is suitable for the algorithm to process. 
The various levels of a categorical variable will be assigned a unique numeric value known as the dummy variable. These dummy variables are handled by the logistic regression model as any other numeric value. So of the approaches used are:
Using the LabelBinarizer from sklearn
Using BinaryEncoder from category_encoders
Using the get_dummies() function of the pandas library
