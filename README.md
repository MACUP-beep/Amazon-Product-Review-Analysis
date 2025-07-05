# DSA Capstone Project
This repository contains my first capstone case study from the DSA Incubator Data Analysis Training Program

# Project Title: Amazon Product Review Analysis - Case Study 1

## Project Overview

This project, "Amazon Product Review Analysis," is Case Study 1 of the DSA Data Analysis Capstone Project. It involves a comprehensive Exploratory Data Analysis (EDA) of Amazon product review data to derive actionable insights for potential sellers or stakeholders. The goal is to understand various aspects of product performance, pricing, discounts, and customer engagement, culminating in an interactive Excel dashboard.

## Data Source

The primary dataset used for this analysis is:
* `Amazon case study File 03072025.xlsx - Amazon Case Study Raw Data.csv`

## Tools Used

* **Microsoft Excel:** For all data cleaning, preparation, analysis (Pivot Tables, calculated columns), and dashboard creation.

## Methodology

The analysis followed a structured approach:

1.  **Data Acquisition and Initial Inspection:** The raw CSV data was imported into Excel. An initial review was conducted to understand column headers, data types, and identify immediate data quality issues.
2.  **Data Cleaning and Preparation:**
    * **Numerical Columns:** `actual_price`, `discount_price`, `discount_percentage`, `rating_count`, `followers`, `reviews`, and `helpful_votes` were cleaned. This involved adding Indian currency symbols, commas, '%' signs, and ensuring correct currency formatting. `discount_percentage` was converted to decimal for calculations.
    * **Date Columns:** `review_date` was cleaned and formatted as a proper date field.
    * **Data Formatting:** The entire dataset was converted into an **Excel Table**. This was crucial for automatically including new calculated columns in Pivot Table data sources and enhancing overall data management.
3.  **Calculated Column Creation:** Several calculated columns were added to enrich the dataset for deeper analysis:
    * `potential_revenue`: `actual_price * rating_count` (to estimate potential sales value).
    * `price_bucket`: Categorizes products into price ranges (`<200`, `200-500`, `>500`).
    * `discount_bucket`: Categorizes `discount_percentage` into ranges (`<10%`, `10-25%`, `25-50%`, `>50%`).
    * `Has_50_Plus_Discount`: A binary flag (`1` or `0`) indicating if `discount_percentage` is >= 50%.

4.  **Analysis with Pivot Tables:** Pivot Tables were extensively used to summarize and analyze the data based on 14 specific business questions. Each Pivot Table was configured to answer a unique aspect of the business problem.


## Key Findings & Actionable Insights

Here are the primary insights derived from the analysis, providing actionable recommendations for Amazon sellers or market analysts:

1.  **Average discount percentage by product category:**
    * **Insight:** `Computers&Accessories` shows higher average discounted prices and significant discount percentages (up to 90%), particularly in subcategories like `PC Headsets` and `Audio&Video Accessories`.
    * **Actionable Insight:** Capitalize on the high discount rates in **`Computers&Accessories`** by promoting these deals more aggressively, especially for subcategories with compelling price points, to drive sales volume.

2.  **How many products are listed under each category?**
    * **Insight:** `Computers&Accessories` is the dominant category with **391 products**, indicating a vast inventory and market presence compared to other top-level categories.
    * **Actionable Insight:** Prioritize inventory management and marketing strategies for **`Computers&Accessories`** to maximize returns from this high-volume category. For smaller categories, explore opportunities for product line expansion.

3.  **What is the total number of reviews per category?**
    * **Insight:** `Electronics` products, especially `Accessories` (over 2M reviews) and `HDMI Cables` (over 1.5M reviews), demonstrate immense customer engagement and trust.
    * **Actionable Insight:** Leverage the high review counts of **`Electronics` accessories and cables** in marketing campaigns to build social proof and attract new customers, potentially cross-promoting with other less-reviewed items.

4.  **Which products have the highest average ratings?**
    * **Insight:** The analysis revealed specific products with very high average ratings, indicating strong customer satisfaction. 
    * **Actionable Insight:** Analyze the characteristics of these **highly-rated products** (e.g., quality, features, value proposition) to apply lessons learned to other products and improve overall customer satisfaction across the catalog.

5.  **What is the average actual price vs the discounted price by category?**
    * **Insight:** Across categories like `Car&Motorbike` and `Computers&Accessories`, there are consistent and significant price reductions when discounts are applied (e.g., `Car&Motorbike` avg. actual: 940 vs. avg. discounted: 499).
    * **Actionable Insight:** Understand the **typical discount depth in each category** to ensure competitive pricing. Deep discounts are a strong customer attraction; ensure these are strategically applied to optimize sales and profit margins.

6.  **Which products have the highest number of reviews?**
    * **Insight:** `AmazonBasics Flexible Premium HDMI Cable` (3-Foot and 6-Feet) and `JBL C100SI Wired In Ear Headphones` are top performers with hundreds of thousands of reviews, showcasing strong market acceptance and brand loyalty.
    * **Actionable Insight:** Study the success factors (e.g., quality, pricing, marketing) of these **highly-reviewed products** to replicate strategies for other products, especially new launches, to accelerate review generation.

7.  **How many products have a discount of 50% or more?**
    * **Insight:** There are **690 products** listed with a discount of 50% or higher. This indicates a substantial number of deeply discounted items on the platform.
    * **Actionable Insight:** These 690 deeply discounted products represent a significant opportunity for attracting price-sensitive customers. Consider dedicated campaigns (e.g., "Flash Sales," "Deep Discount Deals") to highlight these products and drive quick sales volume. This also suggests a highly competitive market for these products, requiring strategic pricing.

8.  **What is the distribution of product ratings?**
    * **Insight:** The majority of products tend to have high ratings, indicating overall positive customer sentiment.
    * **Actionable Insight:** Focus on maintaining high product quality to sustain positive rating distribution. For products with lower ratings, prioritize improvements based on review feedback to lift their performance.

9.  **What is the total potential revenue (actual\_price \* rating\_count) by category?**
    * **Insight:** The `Electronics` category, particularly `Accessories`, represents massive potential revenue (e.g., billions of USD), indicating its immense market size and demand.
    * **Actionable Insight:** Allocate significant resources and strategic focus to the **`Electronics` category**, specifically `Accessories`, to capture the enormous revenue potential and drive overall business growth.

10. **What is the number of unique products per price range bucket?**
    * **Insight:** The distribution of products across price buckets reveals concentrations in certain ranges 
    * **Actionable Insight:** Identify the most populated price buckets to understand market competition. Explore opportunities in less crowded price ranges or strategize to compete effectively within dense segments.

11. **How does the rating relate to the level of discount?**
    * **Insight:** Analysis shows a relationship between average ratings and discount levels. 
    * **Actionable Insight:** high discounts correlate with lower ratings, investigate potential quality issues or customer expectations. high discounts maintain high ratings, this indicates strong value perception that can be leveraged in promotions.

12. **How many products have fewer than 1,000 reviews?**
    * **Insight:** There is indication that a large segment of products that may lack significant customer feedback.
    * **Actionable Insight:** Implement targeted marketing campaigns or "request a review" initiatives for **products with low review counts** to build social proof and improve their visibility and sales potential. Consider offering incentives for early reviews.

13. **Which categories have products with the highest discounts?**
    * **Insight:** `Computers&Accessories` shows the highest individual product discount at **90%**, followed by `Audio&VideoAccessories` at 69%. This signals a highly competitive landscape with aggressive pricing.
    * **Actionable Insight:** For sellers in **`Computers&Accessories`**, offering competitive and deep discounts is essential. Consider bundling or value-added services to differentiate products beyond just price.

14. **Identify the top 5 products in terms of rating and number of reviews combined.**
    * **Insight:** `AmazonBasics Flexible Premium HDMI Cable` (both 3-Foot and 6-Feet) and various `boat Bassheads 100 in Ear Wired Earphones` consistently rank highest based on a combined score of rating and review count. These products successfully combine high customer satisfaction with broad market appeal.
    * **Actionable Insight:** Analyze the features, pricing, and customer feedback of these **top-performing products** to inform product development, marketing, and sales strategies for other products in your catalog.



## Conclusion

This analysis provides a comprehensive overview of Amazon product review data, offering valuable insights into market dynamics, product performance, and customer behavior. The findings and the interactive dashboard can empower sellers to make data-driven decisions regarding pricing, promotions, inventory, and product development to enhance their presence and sales on the Amazon platform.
