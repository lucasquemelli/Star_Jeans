# Star_Jeans

<code><img width="100%" src="https://github.com/lucasquemelli/star_jeans/blob/main/cover%20image/jeans.jpg"></code>

# 1. Business Problems

### Description
---
**Star Jeans** is a fictitious American enterprise whose business model is the sale of jeans by B2C ecommerce. Eduardo and Marcelo are Brazilian businessmen and decided to build a jeans company in the United States of America. The initial idea is the sale of jeans to men. 

**Purpose:** define the products to be sale and their best sale prices.

**Strategy:** keep operational cost and price the lowest as possible in the beginning and enhance them as long as more costumers are won. 

The partners hired a Data Science consultancy company to answer the following questions:

1. What is the best jeans sale price?
2. How many different types of jeans and colors should we choose?
3. What raw materials should we choose to make the jeans?  

The main Star Jeans competitors are the American enterpises H&M and Macys. Firstly, we planned to scrape data from H&M and Macys. However, we found many websites with denied access to their data - Macys was one of them [(Webscraping notebook)](https://github.com/lucasquemelli/ds_ao_dev/blob/main/truereligion_webscraping.ipynb). Thus, we decided to use data from True Religion website instead of Macys. Although we could collect some data, yet it was not possible to collect everything we wanted due to permissions and website layout (that limits scraping).

# 2. Business Assumptions (Formulated Hypothesis)

**Asumptions (hypothesis)** were formulated in order to be tested.

1. **slim_fit** are **20% more expensive** on median than other types of fit. (H&M)
2. **black_no_fade_black** is **the most expensive color**, **around 20%** related to others. (H&M)
3. **ricky_super_t_stitch_straight_jean** is **around 40% more expensive** than the other products. (True Religion)

# 3. Solution Strategy

**Step 01 - Database:** creating a database containing informations such as prices, types, raw materials, color and collection time.

**Step 02 - Schema:** defining the table schema (columns). 

**Step 03 - Infrastructure:** defining the infrastructure (database, csv, API, etc).

**Step 04 - Datapipeline:** creating a datapipeline to extract, transform and load the data. 

**Step 05 - Descriptive Statistics:** Calculating the competitors descriptive statistics related to the price per type, raw material, color and collection time.

# 4. Top 3 Data Insights

# 5. Business Results

# 6. Conclusions

# 7. Next Steps
