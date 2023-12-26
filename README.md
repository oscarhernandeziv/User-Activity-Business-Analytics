# User Activity Business Analytics

## Project Overview

**Objective:** Analyze raw transaction logs to derive business insights for an e-commerce company.

### Data Description
- **Source:** `raw_user_activity` Google Spreadsheet.
- **Contents:** Each row represents an activity or event by a user on the company's website, capturing interactions like viewing product pages, opening shopping carts, or completing purchases.
- **Columns:**
  - `user_id`: Unique customer IDs
  - `event_type`: The type of user activity
  - `category_code`: Category of the product being viewed or purchased
  - `brand`: Company that makes the product
  - `price`: Price of the product (USD)
  - `event_date`: Date of the user activity (YYYY-MM-DD)

## Methodology

### Part 1: Build a Conversion Funnel
- **Objective:** Understand how well the website converts product page views into purchases.
- **Approach:**
  - Created a pivot table in the "conversion_funnel" sheet.
  - Counted unique users at each stage of the funnel (3 stages).
  - Added columns for total conversion rates and conversion rates to the next step.

### Part 2: Prepare Data for Cohort Analysis
- **Objective:** Build acquisition cohorts based on the month of the user’s first purchase and track metrics month by month.
- **Approach:**
  - Isolated purchase events in the "purchase_activity" sheet.
  - Calculated first purchase dates for each user in the "first_purchase" sheet.
  - Created columns for `event_month`, `first_purchase_month`, and `cohort_age` in the "purchase_activity" sheet.

### Part 3: Calculate Retention Rates
- **Objective:** Aggregate purchase data into cohorts and calculate retention rates month by month.
- **Approach:**
  - Grouped data into cohorts in the "cohort_analysis" sheet.
  - Calculated overall retention rates in the "retention_rates" sheet.

### Part 4: Organize and Document the Spreadsheet
- Filled in the "Executive Summary" sheet with results and analysis descriptions.
- Reordered the sheet tabs for logical flow and ease of understanding.
- Formatted spreadsheets for readability.

## Findings

### Conversion Funnel
- **Results Synopsis:** Only 10% of users who viewed the page ended up making a purchase, but 29% of those users got as far as adding an item to their shopping cart.

### Retention Rates
- **Results Synopsis:** The highest retention rate was 6.25% for purchases made one month after the first purchase month of Sept 2020. This is followed by purchases made one month after the first purchase month of Oct 2020 (4.81%) and Dec 2020 (4.43%).

## Conclusion

The analysis of raw user activity logs provides valuable insights into customer behavior, conversion efficiency, and customer retention. By understanding these metrics, the e-commerce company can make informed decisions to optimize the user experience, improve conversion rates, and enhance customer loyalty.

## Live Demo
[Link to Live Demo](https://docs.google.com/spreadsheets/d/1-9YQ7v6T6MpbHv5hJ3_fXRL_7dFKsVMFrNZP-EsU1U8/edit?usp=sharing)
