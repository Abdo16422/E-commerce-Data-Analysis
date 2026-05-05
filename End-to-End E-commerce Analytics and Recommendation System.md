# End-to-End E-commerce Analytics and Recommendation System

##  Overview
This project presents a comprehensive end-to-end data analytics solution for an e-commerce business. 
It focuses on extracting actionable insights from transactional data, understanding customer behavior, 
and building a recommendation system to enhance sales and customer experience.

 Objectives
Analyze sales performance and key business metrics
Understand customer purchasing behavior
Identify product relationships for cross-selling
Segment customers based on value and engagement
Build a recommendation engine for personalized suggestions
Create an interactive dashboard for business monitoring

#  Data Cleaning
- Removed missing values
- Removed negative quantities (returns)
- Removed duplicates
- Converted InvoiceDate to datetime format
- Created TotalPrice = Quantity × UnitPrice

#  Exploratory Data Analysis (EDA)

Key analysis performed:
- Total number of invoices
- Total revenue
- Top-selling products
- Top customers
- Sales by country
- Time-based analysis (daily, monthly, hourly trends)

#  Market Basket Analysis (Apriori)

We used the Apriori algorithm to discover product associations.

### Steps:
- Converted data into basket format
- Applied one-hot encoding (0/1)
- Generated frequent itemsets
- Extracted association rules using lift & confidence

### Key Insights:
- Strong relationships between product variants
- Example:
  - ALARM CLOCK BAKELIKE PINK → RED (confidence = 0.60, lift = 11.39)
  - ALARM CLOCK BAKELIKE PINK → GREEN (confidence = 0.53, lift = 10.87)

# Recommendation System

Built a rule-based recommendation engine using association rules.

### Features:
- Input: Product name
- Output: Recommended products
- Ranking based on lift and confidence

### Example:
If a customer buys:
- ALARM CLOCK BAKELIKE PINK  
The system recommends:
- RED
- GREEN

# Tools & Technologies
  Python (Pandas, NumPy).
  Data Visualization: Plotly
  Machine Learning: Scikit-learn
  Market Basket Analysis: mlxtend (Apriori)


#  Customer Segmentation (RFM Analysis)

Customers were segmented based on:

- **Recency** → How recently they purchased
- **Frequency** → How often they purchase
- **Monetary** → Total spending

### Segments:
- VIP Customers 
- Loyal Customers 
- At Risk Customers 
- New Customers

#  Advanced Customer Segmentation (Machine Learning)

To enhance customer segmentation beyond traditional RFM analysis, we applied an unsupervised machine learning approach 
using K-Means clustering.

We used :contentReference[oaicite:0]{index=0} to automatically group customers based on behavioral patterns.

##  Objective
- Automatically segment customers into meaningful groups
- Discover hidden patterns in purchasing behavior
- Improve marketing and targeting strategies

##  Features Used
We used the RFM features:
- **Recency** → Days since last purchase  
- **Frequency** → Number of transactions  
- **Monetary** → Total spending  

##  Methodology
1. Data preprocessing and feature engineering (RFM)
2. Feature scaling using StandardScaler
3. Determining optimal number of clusters using Elbow Method
4. Applying K-Means clustering
5. Analyzing and interpreting clusters

##  Clustering Results
Customers were grouped into clusters such as:
-  **VIP Customers** → High frequency & high spending  
-  **Loyal Customers** → Regular buyers  
-  **At Risk Customers** → Inactive for a long time  
-  **New / Low-value Customers**

- 
 #  Business Insights
- Some products are strongly correlated (bundling opportunities)
- A small number of customers generate most revenue
- Clear seasonal and time-based sales trends
- Potential for personalized marketing strategies



