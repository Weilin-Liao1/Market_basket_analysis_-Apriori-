# Market Basket Analysis Apriori

## Introduction 
For a long time, marketers are interested in product affinity (similarity of products); for example, coffee and tea are substitutes, so their demand is often negatively correlated. On the other hand, if two products complement each other, their demand is often positively correlated. Hence, price cuts for coffee will usually increase the demand for sugar but decrease tea demand. That is also why marketing specialists are interested in product affinity, as it offers useful information for designing marketing strategies. The market basket analysis offers valuable information to design their marketing strategies, e.g.:

- It can be applied for supermarkets to arrange their shelf space, for retailers and other e- commerce companies to achieve similar benefits.
- It can be used to design promotional plans, such as product bundling or cross-coupon program.
- Market basket analysis with time components is very useful for various marketers to choose
cross-selling products.

Market analysis provides a series of association rules by analyzing transaction data; these rules show which items are purchased together. Every association rule has an antecedent and a consequent; for example, “If a customer buys A, then he/she is likely to buy B”. In this case, A is the antecedent and B is the consequent. However, it is not easy to identify “good” association rules through a single indicator. Therefore, researchers have proposed several different indicators. The most common criteria for evaluating the strength of association rules are support, confidence and lift.

• Support: The proportion of transactions that contains specific items sets, therefore support for combination A, B is (N= total transactions):

Support of AB = P(AB) = frequency (AB) / N

• Confidence: It is the conditional possibility of a decided premise at P(B | A).

Confidence (if A then B)
= P(B|A) = P(AB) / P(A)
= frequency (AB) / frequency (A)

• Lift: Lift is a measure that conquers drawbacks with support and confidence, so it is also called improvement or impact. Consider the association rule "If A then B", the lift is described as:

Lift = P(B|A)/P(B)
= P(AB)/[P(A)P(B)]
=Support / Support(A) x Support(B)

In conclusion, there are three measures for assessing the association rules in market basket analysis. And each one has its benefits and drawbacks, but in general, researchers hope an association rule has high values in all these three criteria. That is, an association with high confidence or support would be interesting rules.

## Apriori algorithm

Apriori and FP Growth are the most commonly used algorithms for market basket analysis. Both algorithms have weaknesses; the FP Growth algorithm takes less time than the Apriori algorithm. However, Apriori algorithm has been found better for the association, and it is less complicated and easier to execute. 
Because of its simplicity, this project will apply Apriori algorithm for market basket analysis. Analyses are done using the library **"Mlxtend"** from the Python programming language.

## Analysis 

Step1. Data Preprocessing and initial data exploration: 

Step 1 includes importing data, exploring the data and implementing data cleansing. 

Step 2. Exploratory Data Analysis:

This step will performing investigations on the cleaned data to discover patterns, visualizations will also be included here.

Step 3. Analysis:

This step will apply Apriori algorithm to the data and discover association rules based on the three criteria (support, confidence and lift). 



## Data and references


**Data:**

**Reference:**
