# Topics
- Low level of differentiation between products available
- Costumer service
- Keeping customers for the long term
- Building brand loyalty

# Tasks
- Determine the client data needed for analysis
- Outline the techniques you'll use to investigate your client's problem
- Explain how i would interpret the outcome
- Write an email to your summarizing your approach

# My Results
Based on PowerCO's hypothesis: customers are sensitive to prices?
- Determine whether price and price changes are associated with churn.
- Identify other factors that predict churn.
- Develop a model that identifies customers at high risk of leaving.
## Data Needed
- Customer data
- Products offered by PowerCO 
- Consumption data
- customer experience data
- competitors pricing (if obtainable)
## Hypotheses
- Customers exposed to larger price increases are more likely to churn.
- Customers paying higher effective prices than similar customers are more likely to churn.
- Customers nearing contract renewal are at greater risk.
- Low-consumption or low-margin customers may respond differently to price changes.
- Complaints or poor service may explain churn
## Techniques
- data wrangling
- eda:
    - compare churn rates across price changes, contract types, consumption levels
- feature engineering
- predictive modeling (start with logistic regression then compare it to tree-based model) + evaluation
- interpretation: rank customers by churn risk and associate it with their margin so the company could target the one who are more likely to leave and the ones who are financially valuable
## Outcome
- price is a strong driver
- service experience is a great factor: improve complaint handling, customer support
- contract timing is important

## Email
Hi,

To understand PowerCo’s customer churn, I would first consider the main reasons a customer might stay with or switch energy providers. These may include price and unexpected price increases, competitor discounts, contract terms, product quality and reliability, customer service, billing accuracy, brand reputation, and customer loyalty. <br>

To analyze these possible causes effectively, I would request the following customer-level data:
- Churn status and date
- Historical prices, tariffs, discounts, and price changes
- Energy consumption and purchasing trends over time
- Products and services used or cancelled
- Contract type, duration, renewal date, and customer tenure
- Customers data
- Customer-service interactions, complaints, and resolution times
- Competitor prices and product offerings, if accessible

<br>
Once the data is available, I would follow the five-step data science process: 
<br>

- Understand the business and frame the problem: Define churn clearly, confirm PowerCo’s objectives, and develop hypotheses about price sensitivity, service quality, product offerings, and other potential churn drivers.
- Exploratory data analysis and data cleaning: Examine customer and pricing patterns, compare churn rates across different groups, and address missing values, duplicates, inconsistent records, and outliers.
- Feature engineering: Create useful measures such as percentage price change, consumption trends, time until contract renewal, complaint frequency, effective price per unit, and products cancelled.
- Modeling and evaluation: Build classification models to predict which customers are likely to churn. I would begin with logistic regression and compare it with tree-based models. Performance would be evaluated using measures such as precision, recall, F1 score, and ROC-AUC.
- Insights and recommendations: Identify the strongest churn drivers and the customer segments most at risk. The findings could guide actions such as targeted pricing offers, improvements to customer service, investment in particular products, or better communication before contract renewal.

<br>
This approach will allow us to test whether price sensitivity is genuinely driving churn while also identifying other factors that may affect customers’ decisions. 

<br>
Best,<br>
Hossam Fadil

# Forage's Result
Hi [Name],

In order to test the hypothesis that churn is driven by the customers’ price sensitivity, we need to model churn probabilities of customers and derive the effect of prices on churn rates.

We would need the following data to be able to build the models:

    Customer data - which should include characteristics of each client, for example, industry, historical electricity consumption, date joined as customer etc
    Churn data - which should indicate if customer has churned
    Historical price data – which should indicate the prices the client charges to each customer for both electricity and gas at granular time intervals


Once we have the data, the work plan would be:

    Define what price sensitivity is and calculate it
    Prepare the data and engineer features 
    Test our hypothesis using a binary classification model (e.g. Logistic Regression, Random Forest) to predict likelihood of churn
    Select the best model based on accuracy metrics and other considerations such as explainability
    With the trained model, extrapolate the extent to which price sensitivity influences churn


Regards,

[Your name]