# Cross Selling Insurance

# Introduction
Salespeople use cross-selling and upselling strategies to generate more business from an existing customer base. In the insurance industry, cross-selling is when you sell additional insurance products to an established client. 

‍Cross-selling insurance allows you to earn additional profit without the cost of searching for new leads. Additionally, you build your client relationship by staying up to date on events and changes in your clients’ lives — which might require new or greater coverage. This can lead to improved client retention. 

‍However, cross-selling must be done the right way. If you aggressively push your clients to purchase products they don’t want or need, you risk losing their business. 

# Business Problem
## Context
An Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.

## What's the problem?
**Build a model to predict whether a customer would be interested in Vehicle Insurance** is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

## The data
The dataset is available on the Kaggle, 
https://www.kaggle.com/anmolkumar/health-insurance-cross-sell-prediction

Now, in order to predict, whether the customer would be interested in Vehicle insurance, you have information about demographics (gender, age, region code type), Vehicles (Vehicle Age, Damage), Policy (Premium, sourcing channel) etc.

### Variable:	Definition
- id:	Unique ID for the customer
- Gender:	Gender of the customer
- Age:	Age of the customer
- Driving_License:	0 : Customer does not have DL, 1 : Customer already has DL
- Region_Code:	Unique code for the region of the customer
- Previously_Insured:	1 : Customer already has Vehicle Insurance, 0 : Customer doesn't have Vehicle Insurance
- Vehicle_Age:	Age of the Vehicle
- Vehicle_Damage:	1 : Customer got his/her vehicle damaged in the past. 0 : Customer didn't get his/her vehicle damaged in the past.
- Annual_Premium:	The amount customer needs to pay as premium in the year
- PolicySalesChannel:	Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.
- Vintage:	Number of Days, Customer has been associated with the company
= Response:	1 : Customer is interested, 0 : Customer is not interested

## Questions to answer
1. Find insights based on the most relevant customers attributes.
2. What percentage of customers are interested in purchasing auto insurance if the sales team
make 20,000 calls?
3. What if the sales team's capacity increases to 40,000 calls?
4. How many calls does the sales team need to make to contact 80% of customers interested in acquiring
a car insurance?

# Solution Planning
1. Conduct an exploratory analysis to find insights about the most relevant customer attributes.
2. Develop a machine learning model to predict the probability of a customer being interested in vehicle insurance.
3. Create a rank of customers more susceptible to purchasing a new product.
4. Define metrics to evaluate different models and choose the best one.
5. Deliver an API capable of sorting customers by interest probability.

## Metric
The evaluation metric for this hackathon is ROC_AUC score.
