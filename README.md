# DynamicPricingEngine
this is a project that explores the concept of dynamic pricing


# Online Research
https://medium.com/@baabak/dynamic-pricing-using-machine-learning-5e882282effe
https://arminkakas.medium.com/building-a-dynamic-pricing-capability-in-under-90-days-10848abd0828
https://arxiv.org/abs/2411.18261
https://medium.com/accelerated-analyst/outsmarting-amazons-pricing-algorithms-with-data-a-consumer-s-guide-to-data-driven-shopping-on-b213e1fe7043
https://medium.com/@informedco/algorithmic-repricing-strategies-cc38ad4728c9
https://www.pragmaticinstitute.com/resources/articles/product/the-amazon-effect-dynamic-pricing-done-right/
https://metricscart.com/insights/edlp-walmart-pricing/
https://taylorwells.com.au/walmart-pricing-strategy/
https://tgndata.medium.com/walmarts-pricing-strategy-a-retail-giant-s-battle-against-e-commerce-titans-37a84b3be901
https://medium.com/@peymaan.abedinpour/how-uber-calculates-your-ride-fare-the-inside-scoop-on-their-pricing-strategy-bee21e050a2f
https://medium.com/system-design/how-uber-surge-price-works-edd898ca3746
https://www.uber.com/en-GB/blog/uber-dynamic-pricing/
https://abovethecrowd.com/2014/03/11/a-deeper-look-at-ubers-dynamic-pricing-model/



# Workflow
1️⃣ Data Overview
Dataset Name: Retail Store Inventory Forecasting Dataset

Dataset Description:

Consists of approximately 70,000 data points capturing daily sales and inventory levels.

Focused on multiple retail stores, providing robust insights into consumer demand patterns and inventory dynamics.

Detailed temporal data allows for granular forecasting and dynamic pricing strategies.

Key Features:

store_id: Identifier for each store.

item_id: Identifier for individual products.

sales: Number of items sold per day.

inventory_level: Inventory available per item per store.

reorder_point: Inventory threshold prompting restocking.

Temporal features: date, week, month.

2️⃣ Problem Statement
Retailers face challenges balancing optimal inventory management and profit-maximizing pricing due to fluctuating demand and inventory levels. Incorrect pricing decisions often result in:

Stockouts: Lost sales and customer dissatisfaction.

Overstocks: Increased inventory holding costs and product wastage.

🎯 Objective:
Create a dynamic pricing solution driven by robust demand forecasting and inventory-level predictions. The model will automatically suggest real-time, profit-optimized prices, incorporating both predicted consumer demand and actual store inventory levels.

3️⃣ Industry Work & Inspiration
📌 Industry Practices:
This project is inspired by real-world retail giants employing inventory-aware dynamic pricing, including:

- Amazon & Walmart: Utilize sophisticated inventory management combined with dynamic pricing models to minimize inventory waste and optimize revenue.

- Zara & Target: Known for rapidly adjusting prices based on inventory and seasonal demand shifts.

🛠 What Makes Our Approach Distinct:
Most existing dynamic pricing systems rely solely on competitive price matching or historical sales.
Our project explicitly integrates inventory forecasting directly into price optimization decisions, bridging inventory management and dynamic pricing strategies—thus providing more holistic recommendations.



4️⃣ Relevance in the Current Business Landscape
In today's highly competitive retail market, accurate inventory and price optimization are more critical than ever due to:

- E-commerce Growth: Increased consumer expectations for personalized pricing and immediate availability.
- Economic Volatility: Rising inflation, supply chain disruptions, and demand uncertainties post-pandemic.
- Sustainability Concerns: Reducing waste through efficient inventory management, directly linked to optimized pricing.

Our solution is timely, addressing these core retail challenges directly and tangibly.



5️⃣ Comprehensive Process Workflow
Clearly laid out step-by-step approach for the project:

✅ Step 1: Data Acquisition & Initial Exploration
Load data and validate integrity.
Initial inspection (missing values, anomalies, consistency).

✅ Step 2: Data Cleaning & Preprocessing
Handling missing values, duplicates, and outliers.
Formatting temporal features clearly (date, week, month).

✅ Step 3: Exploratory Data Analysis (EDA)
Analyze demand trends: daily, weekly, and monthly.
Inventory analysis: turnover rates, restock frequencies, stockouts.
Visualization of sales velocity vs. inventory availability.

✅ Step 4: Advanced Feature Engineering
Demand-Based Features: Sales velocity, elasticity indicators.
Inventory Features: Stock-to-sales ratio, stockout frequency, reorder rate.
Profitability Features: Simulated product cost, margin calculation.

✅ Step 5: Demand Forecasting & Inventory Modeling
Demand Prediction Models:
LightGBM/XGBoost: Predict demand at given pricing and timeframes.
Prophet or SARIMA: Time-series models for robust inventory forecasting.
Evaluate accuracy using RMSE, MAE, MAPE.

✅ Step 6: Pricing Optimization Engine
Define business objective clearly:
Profit maximization while minimizing inventory issues.
Optimization function:

Max Profit = (Optimal Price − Cost) × Predicted Demand
Apply constraints based on inventory thresholds and reorder points.


✅ Step 7: Model Explainability (SHAP)
Provide transparent explanations of key pricing decisions.
Communicate insights on how demand and inventory affect recommended prices.


✅ Step 8: API Deployment (FastAPI)
Serve the finalized model via a REST API.


✅ Step 9: Streamlit Dashboard (Interactive UI)
Front-end allowing non-technical stakeholders easy interaction.

Visuals include:
Predicted price optimization.
Demand and inventory level predictions.
Historical trends, insights, SHAP explainability visuals.
