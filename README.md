# Market-Basket-Analysis
DEFINITION:
Retailers utilize market basket analysis, a data mining approach, to boost sales by better understanding client buying patterns.
Large data sets,such as purchase histories,must be analyzed to identify productgroups and items that are most likely to be bought together.
Question:
Apriori is a statistical algorithm for implementing associate rule mining, that primarily relies on three components: Life, Support and Confidence. Using this algorithm try to find the rules that describe the relation between each of the products that were brought by the customers as described in Dataset Link: Store Data https://drive.google.com/file/d/1y5DYn0dGoSbC22xowBq2d4po6h1JxcTQ/view?usp=sharin

Apriori
Definition: Association rules analysis is a technique to uncover how items are associated to each other. There are three common ways to measure association.

Support. This says how popular an itemset is, as measured by the proportion of transactions in which an itemset appears. In the list below, the support of {apple} is 4 out of 8, or 50%. Itemsets can also contain multiple items. For instance, the support of {apple, beer, rice} is 2 out of 8, or 25%. Support(apple)= 4/8 = 50% support{apple, beer, rice} = 2/8 = 25%

List 1: Apple, Beer, Rice, Ham

List 2: Apple, Beer, Rice

List 3: Apple, Beer

List 4: Apple, Pear

List 5: Milk, Beer, Rice, Ham

List 6: Milk, Beer, Rice

List 7: Milk, Beer

List 8: Milk, Pear

Confidence. This says how likely item Y is purchased when item X is purchased, expressed as {X -> Y}. This is measured by the proportion of transactions with item X, in which item Y also appears. In the above list, the confidence of {apple -> beer} is 3 out of 4, or 75%.

Support(X, Y)/ (Support (X)

One drawback of the confidence measure is that it might misrepresent the importance of an association. This is because it only accounts for how popular apples are, but not beers. If beers are also very popular in general, there will be a higher chance that a transaction containing apples will also contain beers, thus inflating the confidence measure. To account for the base popularity of both constituent items,a third measure called lift is used.

Lift. This says how likely item Y is purchased when item X is purchased, while controlling for how popular item Y is. In Table 1, the lift of {apple -> beer} is 1, which implies no association between items. A lift value greater than 1 means that item Y is likely to be bought if item X is bought, while a value less than 1 means that item Y is unlikely to be bought if item X is bought.

Lift(X -> Y) = Support(X, Y)/ (Support (X) x SupportY))

PROCEDURE:
- Importing Libraries
- Data Preprocessing
- Training Apriori Model on the Dataset
- Visualising the rules
- Displaying the rules in Dataframe
