# Contribution breakdown (%) per member 
- Đinh Gia Bảo - 11220788 - 12.5%
- Lê Trọng Hiệp - 11222286 - 12.5%
- Đào Trọng Hưng - 11222595 - 12.5%
- Nguyễn Lê Anh Minh - 11224245 - 12.5%
- Đỗ Sơn Nam - 11224438 - 12.5%
- Nguyễn Đức Anh - 11220321 - 12.5%
- Bùi Bảo Quang - 11225416 - 12.5%
- Phạm Quốc Việt - 11226910 - 12.5%

# Instructions to run the code
- Run using VScode version 1.100.2.
- Install python, java version 11, correct hadoop version.
- Download the data .csv.

## CUSTOMER SECTIONALIZATION IN E-COMMERCE WITH EDA, RFM MODEL AND K-MEANS CLUSTERING ALGORITHM BY USING PYSPARK IN PYTHON

This project's main goal is to improve consumer segmentation and behaviour analysis by using thorough data analytics methods. The knowledge acquired can then help businesses find new ways to increase income, strengthen marketing efficacy, and foster client loyalty. The study uses K-Means clustering for effective consumer categorisation, RFM (Recency, Frequency, Monetary) analysis, and exploratory data analysis (EDA) to gain first insights and comprehend the properties of the data. PySpark is used to effectively manage data processing and analysis, guaranteeing scalability and excellent performance, because of the dataset's significant quantity and complexity.

## I. Project overview
# 1. Research objectives
The main objective of the project is sectionalizing customers in e - commercea crucial business process that enables organisations to customise their marketing strategies and gain a comprehensive understanding of the requirements, preferences, and behaviours of every customer group to guarantee the best possible service. Consequently, this kind of marketing enables businesses to interact with their customers more effectively. 


Customer segmentation is the act of dividing homogeneous consumers based on shared characteristics is known as customer segmentation. Customers in these segments share characteristics such as gender, age, geography, occupation, and lifestyle, to name a few. The foundation of effective segmentation involves grouping customers and forecasting their potential value to the business. Afterward, create distinct strategies for each group to maximize returns from both high- and low-profit customers.
Businesses can gain a lot from effective consumer segmentation. a some of the main benefits. Above all, it can assist businesses in improving the targeting of their marketing campaigns. Businesses can determine which client segments are most likely to react favourably to particular marketing messages by using segmentation. Campaigns can become more targeted as a result, cutting down on waste and increasing the likelihood of success. Second, client retention and satisfaction can be enhanced by customer segmentation. Consumers are more inclined to stick with a brand if they feel appreciated and understood. Businesses can provide individualised experiences that increase customer satisfaction and retention rates by segmenting their consumer base. Besides, increasing profitability is one of the values that a  successful customer segmentation can provide for businesses. Companies can improve their conversion rates and generate more revenue when targeting customers with suitable offers. For example, a company may use value-based segmentation to identify high-spending customers and offer exclusive promotions, increasing sales and customer loyalty.

# 2. Description of the project
In this project, we use the "E-commerce Customer Behavior and Purchase Dataset" which is a synthetic dataset generated using the Faker Python library. It simulates a comprehensive e-commerce environment, capturing various aspects of customer behavior and purchase history within a digital marketplace. This dataset has been designed for data analysis and predictive modeling in the field of e-commerce. Based on this dataset, we aim to perform EDA (Exploratory Data Analysis) to understand the basic characteristics of the dataset, including distributions, missing values, outliers, and key summary statistics. EDA helps us to get insights into customer purchase behavior, identify patterns, and prepare the data for further analysis. Also, we believe that performing RFM (Recency, Frequency, and Monetary Value) model for this dataset is essential because it can help us to segment the customers based on their purchasing patterns and behavior. To segment customers, data scientists typically create unsupervised machine learning techniques like hierarchical clustering or K-Means clustering. These models are excellent at spotting commonalities among user groups that are frequently missed by the naked eye. Therefore, we can divide our clientele into a variety of categories and provide them with services that are appropriate for them by employing K-Means.

## II. Project methods
# 1. EDA (Exploratory Data Analysis)
# 1.1 Definitions of EDA

Exploratory data analysis (EDA) is used by data scientists to analyze and investigate data sets and summarize their main characteristics, often employing data visualization methods.
EDA helps determine how best to manipulate data sources to get the answers you need, making it easier for data scientists to discover patterns, spot anomalies, test a hypothesis, or check assumptions.
# 1.2 The importance of EDA 
EDA's primary goal is to assist in examining data before drawing any conclusions. It can assist in spotting glaring mistakes, better comprehending data patterns, spotting outliers or unusual occurrences, and identifying intriguing relationships between the variables.

To make sure the findings they generate are reliable and relevant to any intended business outcomes and objectives, data scientists can employ exploratory analysis. EDA also assists stakeholders by verifying that the queries they are posing are pertinent. Standard deviations, categorical variables, and confidence intervals are among the topics that EDA can assist with. EDA's features can be applied to more complex data analysis or modelling, such as machine learning, when it is finished and insights have been obtained.

# 2. RFM Model
# 2.1 Definiton of RFM Model

The RFM model is a widely used marketing analytics tool that helps businesses evaluate and segment their customers based on three key behavioral metrics: Recency, Frequency, and Monetary value. By quantitatively scoring customers on these dimensions, companies can identify their most valuable customers and tailor marketing efforts to maximize engagement and profitability. The underlying principle of the RFM model aligns with the Pareto principle, which suggests that a large portion of business revenue often comes from a relatively small group of customers.
Key Components of the RFM Model
Recency: This metric measures how recently a customer made their last purchase. Customers who have purchased more recently are generally more engaged and have a higher likelihood of responding to marketing campaigns or making repeat purchases. Depending on the nature of the product or service, recency can be measured in units ranging from hours to years.


Frequency: Frequency tracks how often a customer makes purchases within a specific timeframe. Customers with higher purchase frequency demonstrate stronger loyalty and are often the best targets for retention and upselling strategies. New customers with low frequency can be nurtured through targeted campaigns to encourage repeat buying.


Monetary: This dimension quantifies the total amount of money a customer has spent during a defined period. High-spending customers contribute significantly to revenue and are critical for maximizing long-term business value. Understanding monetary value helps prioritize marketing spend and customize offers for different customer segments.
2.2. The importance of RFM Model

RFM analysis plays a crucial role in marketing because it offers a focused approach to understanding where your revenue truly comes from. To distinguish repeat customers from new ones, marketers can design campaigns that enhance customer satisfaction and increase repeat purchases. This segmentation allows businesses to:
- Identify and nurture high-value customers.
- Pinpoint at-risk segments needing re-engagement strategies.
- Discover upsell and cross-sell opportunities based on customer behavior.
RFM analysis is a powerful tool for gaining insights into your customer base. It helps answer critical questions such as:
- Who are your best customers?
- Which customers are at risk of churning?
- Who has the potential to become more valuable?
- Which customers can be effectively retained?
- Who is most likely to respond to engagement campaigns?
It’s crucial to identify and optimize user groups based on behavioral segmentation in order to improve campaign performance. RFM analysis provides a roadmap for personalized marketing. It ensures that the right message reaches the right customer at the right time.

# 2.3 How to make RFM Model
Calculating RFM is easy, and anyone can do it as long as they have access to sales data. We just need columns for customer IDs and each RFM factor. Here are the steps for calculating RFM:
Step 1: Scoring
Each of the three categories will be assigned a score ranging from 1 to 5. As a result, your target market will consist of the clients who add up the most points.

Step 2: Evaluation
You can score each customer separately in each category by reviewing your sales data and customer relationship management (CRM) software after deciding on your scoring strategy. To help you identify which clients are your target demographic, you will then total their aggregate scores to get their final worth. Clients with lower scores might be divided up and targeted with alternative marketing strategies.

Step 3: Boost correspondence with customers
You can prioritise your top clients in your marketing strategy by using the information your RFM research will provide and offer personalized campaigns to entice them to make repeat purchases.

# 3. K-Means clustering algorithm
# 3.1 The Definition of K-Means clustering algorithm 

K-means clustering is a method of vector quantization, originally from signal processing, that aims to partition n observations into k clusters in which each observation belongs to the cluster with the nearest mean (cluster centers or cluster centroid), serving as a prototype of the cluster.
When the centres remain unchanged for two consecutive iterations, the algorithm's stop condition is met. However, people typically cease using the method once an approximate and satisfactory result is obtained because it is exceedingly difficult and time-consuming to acquire a flawless result.

# 3.2 Algorithm implementation steps
Step 1: Specify the number of clusters (k). The first step in k-means is to specify the number of clusters, which is referred to as k. Traditionally researchers will conduct k-means multiple times, exploring different numbers of clusters (e.g., from 2 through 10).

Step 2: Allocate objects to clusters. The most straightforward approach is to randomly assign objects to clusters, but there are many other approaches (e.g., using hierarchical clustering). The 18 objects have been represented by dots on a scatterplot, as seen in the diagram below, where x is shown by the horizontal position of each object and y by the vertical. The objects have been randomly assigned to the two clusters (k = 2), where one cluster is shown with filled dots and the other with unfilled dots.

Step 3: Compute cluster means. For each cluster, the average value is computed for each of the variables. In the plot below, the average value of the filled dots for the variable represented by the horizontal position (x) of the dots is around 15; for the variable on the vertical dimension, it is around twelve. These two means are represented by the filled cross. Or, stated slightly differently: the filled cross is in the middle of the black dots. Similarly, the white cross is in the middle of the white dots. These crosses are variously referred to as the cluster centers, cluster means, and cluster medoids.

Step 4: Allocate each observation to the closest cluster center. In the plot above, some of the filled dots are closer to the white cross and some of the white dots are closer to the black cross. When we reallocate the observations to the closest clusters we get the plot below.

Step 5: Repeat steps 3 and 4 until the solution converges. Looking at the plot above, we can see that the crosses (the cluster means) are no longer accurate. The following plot shows that they have been recomputed using step 3. In this example, the cluster analysis has converged (i.e., reallocating observations and updating means cannot improve the solution). When you have more data, more iterations are typically required (i.e., steps 3 and 4 are repeated until no respondents change clusters).
# 3.3 Elbow method
When employing the k-means approach, the Elbow method is the only way to determine how many centroids should be created. Prior to beginning the k-mean approach, it is crucial to determine the number of k centroids. By examining the deformation function's decrease and determining the elbow point, the Elbow approach assists us in determining the right number of clusters based on the visualisation graph.

The elbow point is where the deformation function's decay rate will fluctuate the most. In other words, adding more clusters won't make the deformation function much smaller from this point on.If the algorithm divides according to the number of clusters at this position, it will achieve the most general clustering properties without encountering overfitting phenomena.

## III. Data Analysis 
# Overview of the Dataset
The "E-commerce Customer Behavior and Purchase Dataset" is a synthetic dataset created with the Faker Python library. It replicates a detailed e-commerce scenario by representing multiple facets of customer interactions and purchasing activities in an online marketplace. This dataset is intended for use in data analysis and predictive modeling related to e-commerce applications. It is well-suited for projects like predicting customer churn, analyzing shopping baskets, building recommendation engines, and identifying market trends.
Variables Description: This section provides a detailed description of the variables included in this E-commerce dataset:
Customer ID: A unique identifier for each customer.
Customer Name: The name of the customer (generated by Faker).
Customer Age: The age of the customer (generated by Faker).
Gender: The gender of the customer (generated by Faker).
Purchase Date: The date of each purchase made by the customer.
Product Category: The category or type of the purchased product.
Product Price: The price of the purchased product.
Quantity: The quantity of the product purchased.
Total Purchase Amount: The total amount spent by the customer in each transaction.
Payment Method: The method of payment used by the customer (e.g., credit card, PayPal).
Returns: Whether the customer returned any products from the order (binary: 0 for no return, 1 for return).
Churn: A binary column indicating whether the customer has churned (0 for retained, 1 for churned).


# 1. Exploratory Data Analysis (EDA)
In the present analysis, the dataset comprises a substantial volume of transactional records (N=250,000) drawn from nearly 50,000 unique customers over a span of more than three years. Such temporal breadth and sample size provide a robust basis for capturing diverse purchasing behaviors and customer heterogeneity, critical for meaningful segmentation.

The descriptive statistics reveal notable variability in key metrics, including product prices, purchase quantities, and total transaction values. The average customer age is approximately 44 years, which is reflective of a mature consumer demographic, and the presence of categorical variables such as product category and payment method enrich the dataset’s multidimensionality.

Importantly, the data quality assessment indicates minimal missingness and an absence of duplicate transactions, reinforcing the reliability of the dataset. However, the presence of missing values in the 'Returns' attribute warrants cautious handling, as this variable may influence customer satisfaction and retention analyses.

Overall, this EDA phase effectively delineates the dataset's structural and statistical properties, establishing a credible groundwork for the application of advanced segmentation techniques like RFM analysis and K-Means clustering. Such preliminary insights are indispensable for tailoring subsequent modeling strategies to the underlying data distribution and ensuring the interpretability and validity of customer segments.

# 2. Revenue Analysis

The chart illustrates the total monthly revenue of the e-commerce platform from January 2020 to mid-2023, with revenue fluctuating primarily between 14 million and 16 million currency units (approximately 140 to 160 billion VND if converted at a rate of 1 unit = 10,000 VND).
Long-term revenue stability: Over nearly three years, monthly revenue remains stable, averaging around 15 million per month, resulting in an accumulated revenue of approximately 270 million units (2.7 trillion VND) in this period. This reflects sustainable growth, a stable loyal customer base, and consistent consumer demand over time.


Short-term economic factors: Minor fluctuations observed in the chart can be attributed to seasonal factors, such as Lunar New Year, Black Friday, or large promotional campaigns. This is typical in the retail sector, reflecting consumer sensitivity to marketing events and seasonal consumption patterns.
A sharp decline of over 50% in revenue during the final month, falling from approximately 15 million to under 8 million currency units (a roughly 53% drop), is a significant warning sign.


From an economic standpoint, this drop could arise from multiple causes: macroeconomic shocks like rising inflation reducing consumers’ purchasing power; customer dissatisfaction or loss of trust due to declining service quality; or increased competition leading to customer churn.

This downturn might also reflect business cycle effects or irregular events such as supply chain disruptions, technical failures, or changes in sales policies.

Economic Significance in Customer Segmentation
- Stable revenue is mainly driven by customers with high purchase frequency and average spending, with an average order value around 2,700 currency units, according to the product category revenue breakdown.

- Specifically, the Books and Clothing categories contribute total revenues of approximately 204.9 million and 204.5 million currency units, respectively, each with about 75,000 transactions. These represent the core customer segment responsible for over 60% of total revenue, indicating frequent purchasing behavior, stability, and broad market penetration.

- Conversely, Electronics and Home categories have lower transaction counts (~50,000 each) but maintain similar average order values (~2,700 units), indicating customers who make higher-value purchases less frequently.

- Customer economics suggest maintaining and growing both segments is vital for sustainable revenue growth:
+ Frequent purchasers (Books, Clothing) stabilize cash flow and maintain operational scale.
+ High-value customers (Electronics, Home) enhance profit margins and provide financial leverage.

# 3. Customer Behavior Analysis
Analyzed data shows that customers fall under two main categories: first time buyers and returning customers. First time buyers constitute only a small portion of the customer distribution, suggesting the business has a steady flow of returning customers. Most customers cluster between three to seven purchases, peaking at four to five transactions. Additionally, the data reveals a declining number of customers as frequency of purchases increases. A small percentage of 3 to 4% of customers make ten or more purchases, constituting the most loyal segment. Customers based on highly differentiated types of behavioral segmentation are divided into groups based on frequency of purchases: low frequency (less than five purchases), mid frequency (five to nine purchases), and hi frequency (ten or more purchases). Mid frequency customers comprise 45% of total customer base, followed closely by low frequency customers at 44%. Although high frequency customers are fewer in number, they tend to provide maximum value, thus making them an important segment for the business. Businesses can identify varying customer range and behavior based on these segments. Loyalty promoting strategies could be implemented for low frequency buyers who are likely to be new or disengaged, while medium frequency buyers represent the core audience who would benefit from retention and upselling efforts.
	+----------------+-----+
	|purchase_segment|count|
	+----------------+-----+
	|   Low Frequency|21632|
	|  High Frequency| 1589|
	|Medium Frequency|26452|
	+----------------+-----+

# 4. RFM Analysis
RFM Analysis segments customers by evaluating three key metrics: Recency (how recently a customer made a purchase), Frequency (how often they purchase), and Monetary value (how much they spend). Each metric is scored on a scale from 1 to 5 based on percentile thresholds, reflecting the customer’s engagement and value level. By combining these scores, customers are classified into meaningful groups such as Champions, New Customers, Loyal Customers, Lost, Cannot Lose Them, and Others. This segmentation reveals important patterns in customer behavior, allowing businesses to tailor marketing and retention strategies effectively to maximize customer lifetime value and business growth.

The RFM analysis classified customers into groups based on their interaction levels and spending value, reflecting their loyalty and growth potential.

- Champions are the most loyal and valuable customers, demonstrating strong engagement through high purchase frequency, substantial spending, and recent transactions. They are the core group of the business, playing a vital role in revenue, and should be prioritized with special care and rewards to ensure retention.

- New Customers have just started transacting, with lower purchase frequency and spending but significant growth potential. Developing strategies to retain and increase purchase frequency for this group will help convert them into loyal customers.

- Loyal Customers exhibit stable behavior with relatively consistent frequency and spending. They represent a sustainable value segment and should be maintained through regular promotions and personalized care to increase their customer lifetime value.

- Cannot Lose Them are customers with high frequency and spending but with less recent purchase activity, indicating a risk of churn. They need reactivation through targeted offers or personalized engagement to bring them back.

- Lost customers show low interaction and spending, with their last purchase occurring a long time ago. This group should be carefully evaluated for retention cost-effectiveness or possibly excluded from marketing campaigns to focus resources on more promising segments.

- Others include customers with unclear or mixed behaviors, requiring further analysis to determine the most appropriate strategy.

Overall, the relationship between these segments illustrates a clear progression cycle: from New Customers → Loyal Customers → Champions, as customer engagement deepens. Meanwhile, the Cannot Lose Them and Lost groups highlight potential pain points and risks of customer loss. Understanding these relationships allows businesses to design targeted care and marketing programs that optimize benefits and maximize long-term value.

- +----------------+--------------+------------------+------------------+------------------+
- |Customer_Segment|customer_count|      avg_monetary|     avg_frequency|       avg_recency|
- +----------------+--------------+------------------+------------------+------------------+
- |       Champions|         17573|20785.405167017583| 7.138906276674444|140.59597109201616|
- |   New Customers|         13840| 7941.732658959538|3.4434971098265894|181.58829479768787|
- | Loyal Customers|          8326|13313.410521258707| 5.026183041076147| 161.9207302426135|
- |            Lost|          5348| 5988.236350037397|2.2025056095736724| 736.1243455497382|
- |Cannot Lose Them|          2658|15876.169676448457| 5.850639578630549| 567.4025583145223|
- |          Others|          1928|10941.792012448133|               4.0| 613.6244813278008|
- +----------------+--------------+------------------+------------------+------------------+

# 5. K-Means Clustering and Visualize Clusters: 

The goal of these and scatter plot is to visualize the relationship between their Recency, Frequency, and Monetary values of customers, and to see how these customers are grouped into different clusters based on the 'prediction' column.

Some insights about these specific clusters:
·       Cluster 0 (High Recency, Low-to-Medium Frequency, Medium Monetary Value): From the Recency vs Frequency plot, this cluster is located in the high Recency, low-to-medium Frequency region, indicating customers who haven’t shopped in a long time (around 2 years) and only purchase occasionally. The Recency vs Monetary plot shows they spend a moderate amount despite their inactivity, and the Frequency vs Monetary plot confirms their low purchase frequency paired with medium spending. These customers are likely at risk of churning, as they haven’t engaged recently and shop infrequently, but their moderate spending suggests they may still have some interest in the products.
·       Cluster 1 (Low Recency, Very High Frequency, Very High Monetary Value): The Recency vs Frequency plot places this cluster in the low Recency, high Frequency region, showing they shop very frequently (around 8-9 times) and recently (within 4-5 months). The Recency vs Monetary plot highlights their high spending paired with recent activity, and the Frequency vs Monetary plot shows a strong correlation between their high frequency and high spending. These are the most valuable customers—VIPs who are highly engaged, shop often, and spend significantly, making them a critical segment to retain.
·       Cluster 2 (Medium Recency, Medium-High Frequency, High Monetary Value): In the Recency vs Frequency plot, this cluster appears in the medium Recency, medium-to-high Frequency area, indicating they shop fairly often (around 5-6 times) but haven’t purchased recently (around 6 months ago). The Recency vs Monetary plot shows their high spending despite the lapse in activity, and the Frequency vs Monetary plot confirms their frequent purchases are tied to high spending. These customers were once highly engaged and valuable, but their recent lack of activity suggests they may be at risk of disengagement, making them prime candidates for re-engagement efforts.
·       Cluster 3 (Medium Recency, Low Frequency, Medium Monetary Value): The Recency vs Frequency plot places this cluster in the medium Recency, low Frequency region, showing they shop infrequently (around 3 times) and haven’t purchased very recently (around 6-7 months ago). The Recency vs Monetary plot shows their medium spending, and the Frequency vs Monetary plot confirms their low purchase frequency with moderate spending. These customers are casual buyers who shop sporadically and spend moderately, indicating potential for growth if their shopping frequency can be increased.
Based on the scatter plot insights and the value of each cluster, let’s assume the following cost allocation for a total marketing budget of 100%:
·       Cluster 0 (High Recency, Low-to-Medium Frequency, Medium Monetary Value): Allocate 8-12% of the cost to this cluster:
These customers are at high risk of churning, but their moderate spending suggests some potential for reactivation, so a small budget is allocated to test re-engagement strategies.
Activities for this cluster: A "Time Capsule Discount" campaign will send personalized messages (e.g., "It’s been 2 years since your last purchase—open this time capsule for a surprise!") offering a 25% discount on their next purchase within 5 days, focusing on past purchase categories, alongside a Virtual "Rediscovery" Tour inviting them to explore new products with a gamified element earning a free gift (e.g., a small accessory) after viewing 3 items, and a "Second Chance" Auction providing exclusive access to discounted overstocked items to encourage a low-risk return.
·       Cluster 1 (Low Recency, Very High Frequency, Very High Monetary Value): Allocate 45-50% of the cost to this cluster:
As the most valuable and engaged customers, this cluster deserves the largest share of the budget to maintain their loyalty and maximize their lifetime value.
Activities for this cluster: A "VIP Star Challenge" will reward customers with "stars" per $500 spent to unlock exclusive perks like early sales access or custom product engraving after 5 stars, a Personalized "Thank You" Box with a curated gift (e.g., sample product and $50 voucher) to celebrate their loyalty, and an Elite Product Co-Creation opportunity where they vote on new product features with a pre-launch discount.
·       Cluster 2 (Medium Recency, Medium-High Frequency, High Monetary Value): Allocate 28-32% of the cost to this cluster:
This group has high spending potential but needs re-engagement due to their recent inactivity, so a significant portion of the budget is allocated to bring them back.
Activities for this cluster: A "Back in Action" Countdown will use a 72-hour timer with tiered discounts (e.g., 15% off within 3 days, 10% within 5 days) to create urgency, an Interactive "Memory Lane" Widget will display past purchases with recommendations and a free upgrade (e.g., free installation), and a "VIP Return Pass" will offer free returns on their next purchase to reduce risk.
·       Cluster 3 (Medium Recency, Low Frequency, Medium Monetary Value): Allocate 12-16% of the cost to this cluster:
These casual buyers have growth potential, but a moderate budget is sufficient to encourage more frequent purchases without over-investing.
Activities for this cluster: A "Frequent Flyer" Rewards program will double points for the next 3 purchases within 30 days (redeemable for a $10 voucher), a Category Explorer Challenge will offer a 10% discount on first purchases in new categories with personalized recommendations, and a "Milestone Surprise" incentive will notify them of nearing a purchase milestone with a mystery gift (e.g., free accessory) upon completion.
These activities are tailored to the scatter plot patterns to maximize engagement and revenue potential across all clusters.
# 6. Payment method analysis:


The chart effectively illustrates the payment preferences of customers across different age groups, highlighting how age influences the choice of payment method in e-commerce transactions. The use of a stacked or grouped bar chart makes it easy to compare the popularity of each payment method within and across age groups, revealing distinct behavioral patterns. For instance, younger customers (e.g., 18-25) may show a preference for digital payment methods like PayPal, while older customers (e.g., 56+) might lean toward more traditional methods like Credit Cards or Cash on Delivery. The chart also allows us to identify which payment methods are underutilized in certain age groups, providing actionable insights for targeted marketing or operational adjustments.
Insights Based on Likely Trends:
·   	Younger Age Groups (18-25 and 26-35) Prefer Digital and Mobile Payments:
It’s likely that customers aged 18-25 and 26-35 show a higher preference for digital payment methods like PayPal or mobile-based payments (if available in the dataset), as seen in the chart where these age groups have a larger proportion of transactions using such methods. This trend aligns with the tech-savvy nature of younger generations, who are more comfortable with online wallets and mobile apps
·   	Older Age Groups (56+) Lean Toward Traditional Methods:
Customers aged 56 and above likely show a preference for traditional payment methods like Credit Cards or Cash on Delivery (if available), as indicated by the chart’s larger proportion of these methods in this age group. Older customers may be less comfortable with digital wallets and prefer methods they’ve used for years, especially for high-value or high-risk purchases.
·   	Payment Method Popularity Varies with Purchase Behavior:
The chart might reveal that payment methods correlate with the type of products purchased by different age groups. For example, younger customers (18-25) using PayPal might be buying lower-cost items like Books or Clothing, while middle-aged customers (36-45) using Credit Cards might be purchasing higher-value items like Electronics or Home products. This can be inferred by cross-referencing the dataset’s Product Category and Total Purchase Amount with age and payment method trends.
·   	Opportunities for Payment Method Optimization:
The chart shows that certain payment methods (e.g., Debit Cards) are underutilized across all age groups, this suggests an opportunity to promote these methods through incentives like discounts or faster checkout processes. Similarly, if older age groups (56+) have low adoption of digital payments like PayPal, the company could offer educational campaigns or tutorials to build trust and familiarity with these methods.

# 7. Gender-based Analysis
Visualize gender preferences 

For Male Customers:
The data shows that Books and Clothing dominate male purchasing behavior, each accounting for approximately 37,000 purchases. This near parity suggests a balanced interest in literary materials and apparel within the male demographic. Following these leading categories, Electronics and Home products attract noticeably fewer purchases, with volumes close to 25,000 each. This substantial drop highlights a marked concentration of male consumer spending on Books and Clothing, with comparatively moderate engagement in Electronics and Home goods.
	For Female Customers:
Purchasing patterns among females differ slightly in priority. Clothing is the most frequently purchased category, slightly exceeding 38,000 purchases, indicating a strong preference for apparel. Books follow closely but with fewer purchases than Clothing, mirroring male customers’ engagement in this category. As with males, Electronics and Home categories hold a consistent but lower position, each with purchase volumes around 25,000. This reflects steady yet reduced female interest in these product areas compared to the leading categories.
	Comparative Insights and Gender Differences:
While both genders engage primarily with the same top categories—Books, Clothing, Electronics, and Home—their relative priorities differ. Males tend to distribute their purchases almost evenly between Books and Clothing, suggesting a dual focus on reading and fashion. In contrast, females demonstrate a clear preference for Clothing over Books, highlighting fashion’s higher importance in their purchasing decisions.
	Purchase Concentration and Distribution:
The marked gap between the top two categories and the remaining ones indicates that consumer purchasing behavior is heavily concentrated. Books and Clothing collectively represent the majority of purchase volumes, while Electronics and Home products, though consistent across genders, account for roughly 30-35% fewer purchases. This disparity points to a focused consumer demand in fewer categories. Electronics and Home categories display similar purchase volumes for both males and females, implying comparable interest levels despite their secondary status. This symmetry suggests these product categories appeal broadly and are less influenced by gender-specific preferences.
# 8. Churn rate 
Visualize churn rate

    Overview of Segments and Churn Rates:
The data presents the total customers and churned customers across six main segments: New Customers, Loyal Customers, Lost, Champions, Others, and Cannot Lose Them. The churn rates are fairly uniform, ranging from 19.34% to 20.24%. The New Customers segment, with 13,840 customers, has the highest churn rate of over 20.24%, indicating that new customers face the greatest risk of leaving, likely due to initial experience or weak brand engagement. Meanwhile, the Cannot Lose Them segment, with 2,658 customers, has the lowest churn rate at 19.34%, reflecting a prioritized retention group with higher value or stronger loyalty.
	In-depth churn rate analysis across segments:
Although Loyal Customers are expected to show the highest loyalty, their churn rate is still around 20.17%, nearly as high as New Customers, signaling concerns over the current retention program effectiveness. The Lost segment, despite its name implying lost customers, also exhibits a churn rate near 20.08%, suggesting overlapping segment definitions or churn measured within a specific timeframe. Champions represent the largest group with 17,573 customers and a churn rate of 19.88%, slightly lower than New and Loyal Customers but still significant, showing that even high-value customers are not fully retained. Others, with 1,928 customers and a churn rate of 19.71%, present a relatively lower churn but with minimal difference compared to Cannot Lose Them.
	Interpretation of the uniform churn rates:
The nearly equal churn rates around 20% across segments indicate systemic retention challenges faced by the company. This uniformity implies that churn drivers may stem from common factors such as customer experience, service quality, market competition, or broader socioeconomic influences rather than segment-specific characteristics. A churn rate close to 20% suggests that on average one in five customers leaves during the period analyzed, signaling a high customer attrition risk. The similar churn rates between New and Loyal Customers raise concerns about the effectiveness of converting new customers into loyal ones, highlighting gaps in seamless customer experience or loyalty programs.
# 9. Seasonal Analysis
    Monthly Revenue Trends
From January to August, revenue remained relatively stable, fluctuating between 57.3 million and 63.2 million. March marked the highest revenue peak at approximately 63.2 million, indicating a possible successful marketing campaign or seasonal sales boost during that month.
However, starting in September, there was a significant and continuous decline in revenue. It dropped from around 62.4 million in August to just 45.7 million in November. Although December saw a slight rebound to 46.8 million, it was still well below the earlier part of the year.
This downward trend in the last quarter (Q4) could indicate declining customer interest, reduced marketing activity, or external factors such as economic changes or seasonality impacting performance.

    Monthly Transaction Count
The number of transactions followed a similar pattern to revenue. From January through August, transaction counts stayed consistently high, ranging from 21,000 to 23,000+. March again led with the highest transaction volume at 23,107, reinforcing its strong performance overall.
In contrast, from September to December, the number of transactions dropped sharply, reaching a low of 16,726 in November. December showed a slight increase, but the level remained significantly lower than the earlier months.
This decline aligns with the revenue trend and suggests a drop in customer engagement or purchase frequency during the last quarter.

# 10. Advanced Analytics
Customer Lifetime Value (CLV):
+-------+-----------------+
|summary|    Estimated_CLV|
+-------+-----------------+
|  count|            47982|
|   mean|95524.30302902608|
| stddev|355662.0109466176|
|    min|   2473.998046875|
|    max|      3.6330687E7|
+-------+-----------------+
The CLV was calculated using a customer’s average order value multiplied by their purchase frequency and annualized over 12 months. This method gives a forward-looking estimate of how much value each customer brings in a year. The results show a wide range, from as low as around 2,474 to as high as over 36 million. The high standard deviation indicates that most customers have moderate value, while a few contribute significantly more, creating a skewed distribution.
Top 10% Revenue Contribution:
Top 10% customers contribute 11.64% of total revenue
Interestingly, the top 10% of customers contribute only 11.64% of total revenue. This is relatively low, especially compared to industries where the top 10% often drive 30–50% of revenue. It suggests that while the business has some high-value customers, revenue is more evenly spread out. There’s an opportunity here to focus on increasing revenue from the top segment through loyalty programs, premium offers, or exclusive experiences.
Overall Return Rate:
+-------------------+-------------------+
|overall_return_rate|    return_rate_std|
+-------------------+-------------------+
| 0.4963391210587942|0.28573203619410803|
+-------------------+-------------------+
The average return rate across all customers is 49.63%, meaning almost half of the purchases are returned. This is a very high figure and could have a serious impact on profitability. A high return rate might indicate issues such as poor product fit, misleading descriptions, or low customer satisfaction. It calls for a closer review of the return process and product-related feedback.
High Return Behavior:
Customers with >10% return rate: 43220 (87.01%)
Further analysis shows that 87.01% of customers have a return rate higher than 10%, making high return behavior a widespread issue rather than a case of a few problematic shoppers. This highlights an urgent need for action, such as improving product images and details, offering better size guidance (if applicable), or even using predictive tools to reduce return risk. Reducing returns even slightly could lead to substantial profit recovery.

## CONCLUSION
# E-commerce Data Analysis Summary and Recommendations
To fully summarize, a thorough grasp of our shoppers is essential for shaping sound business tactics. In this project, our group relied on the RFM framework—recency, frequency, and monetary value—to profile buying habits, then ran K‑means clustering and checked the Elbow plot to choose an appropriate demographic. By combining the models, clear spending patterns and separated customers into data‑driven segments have been revealed. The findings give management a practical view of who buys often, who spends the most, and other segments of customers. With that knowledge, the store can create personalized loyalty offers, focus promotions on high‑potential segments, and use its marketing budget more efficiently.

Although extremely careful analyses have been carried out, there are some success factors that businesses should explore further. First, implementation of the aforementioned methods should be strictly data-driven to ensure accurate and precise analysis. Second, it is essential to continuously monitor the customer information for optimization. Cross-functional collaboration between data, marketing and business departments should also be placed in high regard. Finally, based on performance metrics, the board of directors should regularly review and make adjustments of strategies.

To ensure that business will thrive in the future, our group has come up with some recommendations. The project has meticulously analyzed the data of shoppers but has yet to take stakeholders into consideration, so the next thing to do is to present findings to this group. Resources are also crucial for future implementation; securing them would be undoubtedly important. To make sure that data is collected carefully, tracking and monitoring systems will have to be set up. Finally, iterative improvements and scaling should also be planned for smooth and accurate future analysis.
