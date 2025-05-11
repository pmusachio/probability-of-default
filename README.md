# Probability of Default
>WORK IN PROGRESS...

<br/>

## Probability of Default (PD) Explained Simply

The **Probability of Default (PD)** is the chance that a borrower will fail to repay their loan. Simply put, it's the likelihood that they won't be able to make the required payments.

For banks and other lenders, the PD is a key measure of credit risk. **A high PD indicates a greater risk that the lender won't get their money back.** As a result, loans with a higher PD often come with higher interest rates or require more collateral. If the PD is too high, the lender might even reject the new loan application.

**Key takeaways in simple terms:**

* **PD:** The likelihood a borrower won't repay.
* **High PD:** Higher risk for the lender of not recovering the loan.
* **Consequences of high PD:** Higher interest, more collateral needed, or loan denial.

<br/>

<h3>↑ P(default) = ↑ Interest Rate %</h1>

<br/>

## How Probability of Default (PD) is Estimated

To calculate the likelihood that someone will not repay a loan (PD), banks use **statistical models**. These models analyze various factors about the person, such as:

* **Credit score:** A summary of their payment history.
* **Income:** How much money they earn.
* **Debt-to-income ratio:** How much they owe compared to what they earn.

These models use past data and information about the customer to try and predict the probability that they will fail to repay the loan in the future.

```python
from sklearn.linear_model import LogisticRegression
import pandas as pd

df = pd.read_csv('<path_to_default_dataset>')

features = ["income", "age", "payment_delays", "credit_score"]
label = 'default'

X = df[features]
y = df[label]

model = LogisticRegression()
model.fit(X, y)

predictions = model.predict_proba(X_new)
```

## The Importance and Calculation of Probability of Default (PD)

In short, the chance of a customer not repaying (PD) is very important for lenders. It helps them assess the risk of each loan. One of the most common ways to calculate this chance is by using a type of model called **logistic regression**, which is a classification algorithm.
