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

## Case description 

This project is part of my master thesis, "Integrated Approaches for Developing Market Entry Strategies: A Case Study of Olympus OEM Businesses in the Italian Market." Olympus is a worldwide leading optical and digital precision technology manufacturer, providing medical systems, digital cameras, and scientific solutions. In the thesis, market basket analysis is implemented for Olympus, focusing on OEM microscope businesses. 

However, This master thesis is not to be made available to the public. The information contained is to be treated confidentially; therefore, I will apply another dataset in this project (see the later part, "Data" for more details). 

## Apriori algorithm

Apriori and FP Growth are the most commonly used algorithms for market basket analysis. Both algorithms have weaknesses; the FP Growth algorithm takes less time than the Apriori algorithm. However, Apriori algorithm has been found better for the association, and it is less complicated and easier to execute. 
Because of its simplicity, this project will apply Apriori algorithm for market basket analysis. Analyses are done using the library **"Mlxtend"** from the Python programming language.

## Analysis 

Step1. Data Preprocessing and initial data exploration: 

The first step includes importing data, exploring the data and implementing data cleansing. 

Step 2. Exploratory Data Analysis:

This step will investigate the cleaned data to discover patterns; data visualizations will also be included here.

Step 3. Analysis:

This final step will apply the Apriori algorithm to the data and discover association rules based on those three criteria (support, confidence, and lift). 

## Data and references

**Data:**

It is usually to find real sales data sets in public as they are usually proprietary. However, the <a href="https://archive.ics.uci.edu/ml/datasets/online+retail "> UCI Machine Learning Repository</a>  produced a data set containing actual transactions in 2010 and 2011. This data set is maintained on their website and can be found under the title "Online Retail". This is a multinational data set that contains all the transactions that occurred between 01/12/2010 and 09/12/2011 for non-store online retail registered in the UK. The company mainly sells unique all-occasion gifts. Many of the client companies are wholesalers.

**Reference:**

- Blattberg, R. C., Kim, B.-D., & Neslin, S. A. (2008). Database Marketing Analyzing and Managing Customers. Springer New York.
- Bayardo, R. J., & Agrawal, R. (1999). Mining the Most Interesting Rules. Proceedings of the Fifth ACM SIGKDD International Conference on Knowledge Discovery and Data Mining - KDD '99, 145-154. doi:10.1145/312129.312219
- Al-Maolegi, M., & Arkok, B. (2014). An Improved Apriori Algorithm For Association Rules. International Journal on Natural Language Computing, 3(1), 21-29. doi:10.5121/ijnlc.2014.3103
- Dhanabhakyam, M., & Punithavalli, M. (2011). A Survey on Data Mining Algorithm for Market Basket Analysis. Global Journal of Computer Science and Technology, 11(11).
- Hossain, M., Sattar, A. H., & Paul, M. K. (2019). Market Basket Analysis Using Apriori and FP Growth Algorithm. 2019 22nd International Conference on Computer and Information Technology (ICCIT). doi:10.1109/iccit48885.2019.9038197
- Harikumar, S., & Dilipkumar, D. U. (2016). Apriori algorithm for association rule mining in high dimensional data. 2016 International Conference on Data Science and Engineering (ICDSE). doi:10.1109/icdse.2016.7823952
