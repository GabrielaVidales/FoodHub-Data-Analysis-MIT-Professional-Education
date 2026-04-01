# FoodHub Data Analysis: Data Science Capstone Project

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Pandas](https://img.shields.io/badge/pandas-1.3+-150458.svg)](https://pandas.pydata.org/)
[![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📋 Project Overview

This project was developed as part of the **MIT Professional Education - Applied AI & Data Science Program**, a comprehensive diploma program focused on practical applications of artificial intelligence and data science in business contexts.

The analysis focuses on **FoodHub**, a New York-based food aggregator company. The goal is to analyze order data to understand restaurant demand, evaluate operational performance (preparation and delivery times), measure customer satisfaction, and provide data-driven recommendations to enhance business operations and customer experience.

The project demonstrates end-to-end data science skills, including data cleaning, exploratory data analysis (EDA), statistical analysis, and generating actionable business insights.

## 🎯 Key Objectives

*   **Demand Analysis:** Identify top-performing restaurants and cuisine types, distinguishing between weekday and weekend patterns.
*   **Operational Evaluation:** Calculate and analyze preparation and delivery times, identifying potential bottlenecks.
*   **Customer Satisfaction:** Explore relationships between customer ratings and factors such as order cost and delivery time.
*   **Business Insights:** Generate concrete recommendations to improve customer experience, optimize operations, and maximize revenue.

## 📊 Dataset Description

The analysis uses `foodhub_order.csv`, containing 1,898 orders with the following attributes:

| Column | Description |
|--------|-------------|
| `order_id` | Unique order identifier |
| `customer_id` | Customer identifier |
| `restaurant_name` | Name of the restaurant |
| `cuisine_type` | Type of cuisine ordered |
| `cost` | Order cost (USD) |
| `day_of_the_week` | Weekday or Weekend |
| `rating` | Customer rating (1-5) or "Not given" |
| `food_preparation_time` | Preparation time (minutes) |
| `delivery_time` | Delivery time (minutes) |

## 🛠️ Technologies & Libraries

*   **Language:** Python 3.8+
*   **Environment:** Google Colab / Jupyter Notebook
*   **Data Manipulation:** `pandas`, `numpy`
*   **Visualization:** `matplotlib`, `seaborn`
*   **Statistics:** Built-in Python statistics libraries

## 🔍 Key Findings

The analysis revealed several critical insights:

1.  **Weekend-Driven Demand:** Orders are significantly higher on weekends, representing peak demand periods.
2.  **Cuisine Concentration:** American cuisine dominates, with **415 weekend orders**, indicating clear core categories.
3.  **Restaurant Concentration:** A small group of restaurants drives most volume. **Shake Shack** leads with **219 orders**, followed by The Meatball Shop (132), Blue Ribbon Sushi (119), Blue Ribbon Fried Chicken (96), and Parm (68).
4.  **Operational Performance:**
    *   Average preparation time: **27.37 minutes**
    *   Average delivery time: **24.16 minutes**
    *   **~10.54%** of orders exceed **60 minutes** total (preparation + delivery)
    *   Weekday deliveries are **~6 minutes slower** than weekends (28.34 min vs. 22.47 min)
5.  **Customer Satisfaction:**
    *   **736 orders (39%)** have no rating, limiting satisfaction analysis
    *   Rated orders show predominantly positive feedback (4-5 stars)
    *   Near-zero correlation between ratings and cost/delivery time suggests other factors (food quality, accuracy) drive satisfaction
6.  **Revenue Structure:** Under the tiered commission model (25% for orders >$20, 15% for orders >$5), total net revenue is **$6,166.30**. Approximately **29.24%** of orders exceed $20, representing a valuable premium segment.
7.  **Promotion-Eligible Restaurants:** Restaurants meeting criteria (>50 ratings, avg rating >4) are:
    *   The Meatball Shop (avg rating: 4.51)
    *   Blue Ribbon Fried Chicken
    *   Shake Shack (133 ratings)
    *   Blue Ribbon Sushi

## 💡 Strategic Recommendations

### A) Demand & Growth Strategy
*   **Weekend-focused campaigns:** Concentrate major promotions and featured placements on weekends to maximize conversion.
*   **Price-based segmentation:** Offer bundle deals for the value segment (<$20) to increase basket size, while curating "Premium Picks" collections for the >$20 segment.
*   **Cuisine visibility:** Prioritize top cuisines (American, Japanese) in discovery features while rotating low-volume cuisines to test demand growth.

### B) Restaurant Partnerships & Promotions
*   **Support key partners:** Provide operational support to high-volume restaurants (e.g., Shake Shack) and explore co-marketing agreements.
*   **Data-driven promotions:** Use the established criteria (>50 ratings, avg rating >4) to select restaurants for ad placements and "Recommended" badges, ensuring quality and reliability.
*   **"Rising Stars" program:** Give controlled visibility to high-rated but low-sample restaurants to diversify supply without compromising customer experience.

### C) Operational Optimization
*   **Target 60+ minute orders:** Analyze root causes (preparation vs. delivery delays) and implement corrective actions with restaurants and couriers.
*   **Improve weekday delivery:** Increase courier supply during weekday peak windows (lunch/dinner) and optimize routing to reduce the 6-minute gap compared to weekends.

### D) Data Quality Enhancement
*   **Reduce unrated orders:** Implement post-delivery nudges (one-tap rating prompts) or small incentives (points, discounts) to increase rating response rates, enabling more reliable satisfaction analysis.

---

## 👩‍💻 Author

**Gabriela Yasmin Vidales Ayala**  
*Applied AI & Data Science Program*  
MIT Professional Education

This project was developed as a capstone assignment for the MIT Professional Education diploma program, demonstrating applied data science skills in a real-world business context.

---

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
