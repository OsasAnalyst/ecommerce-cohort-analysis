# Executive Summary: Decoding Customer Loyalty for UK Retailer Brand (2010-2011)

## High Customer Churn Threatens Growth
This UK-based retailer (with 90% of sales from the UK market) faced a critical challenge: **70-80% of new customers never made a second purchase within 3 months**. Despite strong one-time sales (e.g., £1.16M in November 2011), the business was leaking long-term revenue due to poor retention—especially after holiday peaks like December 2010, where only **26.5% of customers returned after 12 months**.

To diagnose the issue, I analyzed the retailer's own sales data (Dec 2010 - Dec 2011), focusing on:

### Customer Purchase Patterns
- **Top-selling items** were low-cost crafts (e.g., "PAPER CRAFT, LITTLE BIRDIE" - 80,995 units) and home goods ("MEDIUM CERAMIC TOP STORAGE JAR" - 77,916 units), suggesting a **price-sensitive, hobbyist customer base**.
- **Sales volatility**: Revenue dropped **55%** from November to December 2011, indicating over-reliance on seasonal buyers.

### Cohort-Specific Retention
- Built a retention heatmap revealing stark drop-offs:
  - **December 2010 cohort**: Only 36.6% returned in Month 1, dwindling to 26.5% by Month 12.
  - **Summer 2011 cohorts (e.g., June)**: Worse retention—just **9.5%** of customers stayed past Month 6.

## The Solution: Targeted Actions for This Retailer
### Fix the "Post-Holiday Churn"
- December 2010's cohort had the highest 12-month retention (26.5% vs. average <10%).  
**Opportunity**: Launch a **"New Year Craft Challenge"** email series (featuring top products like the birdie craft) to extend engagement beyond gifting season.

### Stabilize Off-Peak Sales
- Low retention in non-holiday months (e.g., April-August) suggests **lack of recurring demand**.  
**Solution**: Introduce subscription options for high-volume items (e.g., "Cake Cases" sold 33,669 units).

### Leverage the UK Market
- Since 90% of sales are domestic, **partner with UK-based crafting influencers** to promote repeat purchases of best-sellers.

## Key Metrics
| Metric | Value |
|--------|-------|
| Peak Monthly Sales | £1.16M (Nov 2011) |
| Worst Retention | 9.5% (June 2011 cohort) |
| Top Product | "PAPER CRAFT, LITTLE BIRDIE" (80,995 units) |
| UK Market Share | 90% of total sales |


---

## Data Preparation

### Raw Data
- Used the UK retailer's sales records from December 2010 to December 2011
- Started with over 500,000 transactions

### Cleaning Steps
1. **Removed incomplete data**:
   - Deleted orders missing product names or customer IDs

2. **Fixed incorrect entries**:
   - Removed canceled/returned orders (negative quantities)
   - Deleted transactions with "Unspecified" country

3. **Standardized formats**:
   - Fixed date formats for proper analysis
   - Made sure customer IDs were consistent whole numbers

### Final Dataset
- Cleaned data ready for analysis: ~400,000 valid transactions
- Focused on key details: purchase dates, customer IDs, products, quantities, and countries


---


## Exploratory Data Analysis (EDA)

### 1. Monthly Sales Trends (2010-2011)

<img width="1013" height="485" alt="Monthly sales trend (2010-2011)" src="https://github.com/user-attachments/assets/26dbfd13-eab7-41d2-89ab-693f57110767" />


**Key Insights:**
- **Peak Season**: November 2011 was the strongest month (£1.16M), likely due to holiday shopping
- **Biggest Drop**: 55% sales decrease from November to December 2011 suggests poor post-holiday retention
- **Growth Pattern**: Steady increase from April to November, indicating seasonal business nature


### 2. Top Selling Products

<img width="1023" height="576" alt="Top 10 best selling products" src="https://github.com/user-attachments/assets/7a809925-82ac-44fa-9d6a-ab2e30bc624b" />


**What the Data Shows:**
1. **Craft Dominance**: Paper crafts and ceramic jars lead sales (80k+ units each)
2. **Gift Items**: 6/10 top products are decorative (e.g., bird ornaments, light holders)
3. **Price Sensitivity**: All bestsellers are low-cost items (<£20 based on market research)

**Business Implication:**  
The retailer should focus on promoting complementary products to craft buyers (e.g., "Customers who bought paper birdie also bought...").


### 3. Geographic Sales Distribution

<img width="989" height="468" alt="Top 10 Countries by sales" src="https://github.com/user-attachments/assets/aef21730-ff72-44d7-b929-646ba35c2239" />


**Market Breakdown:**
- **UK Dominance**: 90%+ of total sales (not shown in graph but confirmed in data)
- **Secondary Markets**: Netherlands and Ireland (EIRE) are top international buyers
- **Opportunity Gap**: Minimal presence in major EU markets like Germany/France

**Recommendation:**  
Test localized marketing in Netherlands/Ireland before expanding to other EU countries.

---


## Cohort Analysis Findings


### Customer Retention Patterns
<img width="953" height="468" alt="Customer retention rate by cohort" src="https://github.com/user-attachments/assets/1920072a-8a20-4ee2-baa0-61e2852d9f4a" />


**Key Observations:**
1. **Best Performing Cohorts:**
   - December 2010: 36.6% returned after 1 month, 26.6% after 1 year
   - October 2011: 24% Month 1 retention (better than average)

2. **Worst Performing Cohorts:**
   - March-April 2011: Only 15-21% returned after 1 month
   - November 2011: Worst retention (just 11.1% came back)

3. **Seasonal Pattern:**
   - Holiday buyers (Dec) stayed longer than summer buyers
   - Retention drops fastest in first 3 months

### Customer Spending Trends
<img width="953" height="470" alt="Average Revenue per customer by cohort" src="https://github.com/user-attachments/assets/093ccea4-3bba-4c1d-b372-87f6bd045e48" />


**Spending Insights:**
- December 2010 customers spent most (£33-£50 per month)
- Later 2011 cohorts spent less (£15-£20 on average)
- Big spenders tend to stay longer (see Dec 2010 vs others)

## Recommendations

### Immediate Actions
1. **Save the Holiday Buyers**
   - Launch "New Year Projects" email series for December cohorts
   - Offer bundle deals on top crafts (paper birdie + paint sets)

2. **Fix the First 90 Days**
   - Create onboarding program for new customers:
     - Week 1: Thank you + crafting tips
     - Month 1: Exclusive beginner project
     - Month 3: Loyalty reward offer

3. **Boost Summer Sales**
   - Run "Summer Craft Challenge" for low-retention months
   - Partner with UK parenting blogs for seasonal promotions

### Long-Term Strategies
- Start subscription service for top products (cake cases, storage jars)
- Develop intermediate-level craft kits to keep customers engaged
- Test postcard reminders for UK customers (low tech, high touch)

## Limitations

1. **Data Constraints**
   - Only covers 13 months (limited year-over-year comparison)
   - No customer demographics (age/location details missing)

2. **External Factors**
   - Unknown marketing changes during 2011
   - Can't track why customers left (no survey data)

3. **Technical Limits**
   - Can't see individual customer paths
   - No price change history available

## Future Work

1. **Deepen the Analysis**
   - Add 2012 data to compare year-over-year trends
   - Study product categories (not just individual items)

2. **New Research Questions**
   - Why did December cohorts perform better?
   - What makes customers spend £50+ vs £15?

3. **Business Experiments**
   - Test retention ideas with small customer groups
   - Measure impact of new onboarding program

4. **Data Improvements**
   - Collect customer feedback at checkout
   - Add website browsing behavior data


## Let’s Work Together

This analysis revealed actionable insights about customer retention and spending patterns—but every business has unique challenges. I’d love to help you:  
- **Improve retention** for your specific customer base  
- **Design targeted campaigns** based on cohort behavior  
- **Build custom analytics** to track what matters most  

🔗 **Connect with me on LinkedIn**:  
[Osaretin Idiagbonmwen](www.linkedin.com/in/osaretin-idiagbonmwen-33ab85339)  

📩 **Open for**:  
- Freelance data analysis projects  
- Collaborative research  
- Short-term consulting engagements  

*Let’s turn your data into growth strategies!*  
