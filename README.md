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

**Hypothesis 1:** slim_fit are 20% more expensive on median than other types of fit. (H&M)

**False.** H&M Slim fit products are 9.64% and 25% cheaper (on average and on median, respectively) than other fits. They are the most available fit in the website. We may increase the price.

**Hypothesis 2:** black_no_fade_black is the most expensive color, around 20% related to others. (H&M)

**True.** Although it is the most expensive color, H&M Black no fade black products are 37% and 25% more expensive (on average and on median, respectively) than other colors. It is one of the least available product in the store. We may try to put more products with this color available for purchase.

**Hypothesis 3:** ricky_super_t_stitch_straight_jean is around 40% more expensive than the other products. (True Religion)

**True.** It is true, yet it is more than 40%. True Religion Ricky super t stitch straight jean products are 53% and 50% more expensive (on average and on median, respectively) than other products. It is the first most available products on the website. We may become it the most available and observe a profit increase.

# 5. Business Results

In this section, the business problems set by Star Jeans's businessmen was solved and discussed.

1. What is the best jeans sale price?

This question must be answered based on fit and color, for example. For the most fits, a median price around USD 30.00 was found. For color, this value varies too much and must be answered based on any specific color. We have a boxplot with different colors and their prices on section 2.

2. How many different types of jeans and colors should we choose?

We found 5 fits and 16 colors in the H&M website. This combination may result in 80 different types of jeans. The three most frequent fit were slim, skinny and loose. We may achieve a profit between 9 and 25% by using slim fit (based on previous section). The most frequent colors were denim blue, black, light denim blue and dark denim blue. Although the previous colors were the most frequent, the most profitable color is black no fade black (between 25 and 37%). We may choose this color as the most available on the website. For True Religion we could not collect this type of data.

3. What raw materials should we choose to make the jeans?

We found 6 materials for the jeans, they were: cotton, polyester, spandex, lyocell, rayon and elastomultiester. However, the most correlated materials with the price, based on Pearson correlation coefficient, were elastomultiester, lyocell and rayon.

# 6. Conclusions

We found a range between USD 20 and USD 50 for the jeans, yet this values varies with fit and color. We must specify fit and color to set a better price. The most frequent colors were denim blue, black, light denim blue and dark denim blue. Although the previous colors were the most frequent, the most profitable color is black no fade black (between 25 and 37%). We also found 6 materials for the jeans, they were: cotton, polyester, spandex, lyocell, rayon and elastomultiester. However, the most correlated materials with the price, based on Pearson correlation coefficient, were elastomultiester, lyocell and rayon. 

# 7. Next Steps

Since we have few data because we could not collect data by automation (website layout changes constantly and the webscraping code must be changed), a suggested next step is to find a website which layout does not vary too much. Thus, we may collect a big quantity of data and try to use a Machine Learning model to make business decisions.
