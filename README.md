# 📦 Amazon Sales Analytics and Data Science Models (CS661 Project - IIT Kanpur)

This project is a deep-dive into **eCommerce transaction data** from Amazon (sourced via Kaggle), with a combination of:

- 🧠 Machine Learning models
- 📊 Customer analytics
- 📈 Forecasting
- 🔍 Recommendation engines
- 🌐 Market basket analysis
- 🧬 RFM-based segmentation
- 📡 Visualization-ready outputs

All core logic is implemented in a **single Jupyter Notebook**, used for data preparation and exported for advanced **interactive visualizations** (for CS661 coursework). I have not added the dataset file as it will be very large for uploading. Attaching project Report for final Visuals made using D3 Library, Folium and React with a python (Fast-API) based Backend hosted for temporary period of semester. 

---

## 📁 Dataset

- **Source**: [Kaggle - Amazon Sales Data (public domain)](https://www.kaggle.com/)
- **Content**:
  - Transactional records
  - Product IDs & categories
  - Customer IDs & geolocation
  - Timestamps, quantities, and prices

---

## 🎯 Objectives

- Build a mini decision-support tool based on Amazon sales data
- Extract actionable insights for:
  - Business intelligence
  - Personalized marketing
  - Inventory and sales forecasting

---

## ⚙️ Techniques & Models Used

| Area                       | Technique/Algorithm                                           | Output/Goal                                |
|----------------------------|---------------------------------------------------------------|---------------------------------------------|
| 🛒 Product Recommendation   | **Collaborative Filtering** (user-item, Item-Item basesd)    | Recommend products to users                 |
| 📊 Market Basket Analysis   | **Apriori Algorithm**, **FP-Growth**                         | Find frequent itemsets and rules            |
| 🔁 Association Rules        | Lift, Confidence, Support                                    | Visualize product association strength      |
| 🌉 Sankey Plot Prep         | Category flows                                               | Track user-product-category interaction     |
| 📈 Sales Forecasting        | Time Series Aggregation, Pre-trained Model-Prophet           | Predict future sales volume/trends          |
| 📆 Cohort Analysis          | Retention metrics based on join month                        | Analyze lifecycle and loyalty               |
| 👥 Customer Segmentation    | **RFM (Recency, Frequency, Monetary)**                       | Segment users into High, Medium, Low tiers  |
| Topic Mining                | Using Latent Dirchilet Allocation (LDA) and NLP text preprocessing, Tsne plots   | Understand what users are talking about, issues and sentiment |

---

## 🧠 Notable Implementations

- **Collaborative Filtering**:
  - Constructed a user-product matrix
  - Used cosine similarity to recommend similar items

- **Market Basket**:
  - Preprocessed transactions to create binary item matrices
  - Applied Apriori and FP-Growth (using `mlxtend`)

- **Topic  Mining and Sentiment Analsyis**:
  - Cleaned Text reviews data and perform tokenzation using different vectorization methods
  - Applied Latent Dirchielt Allocation mdethods for finding key topics in the reviews and also get sentiment idea of reviews acroass categories
- **RFM Segmentation**:
  - Computed Recency, Frequency, and Monetary scores
  - Clustered customers into segments using score thresholds

- **Cohort Retention**:
  - Monthly cohorts based on first purchase
  - Computed retention rates over months
- **Sales Forecasting**:
  - Grouped data by date
  - Applied rolling averages, basic forecasting and pre-trained model based forecasting

---

## 🖼️ Visual Outputs

These analytics were used to power the **CS661 Visualization Project**, including:
- 🎢 Topic Mining T-SNE plot of Reviews embeddings from higher dimensional space to 3D space and see its clustering happening fo similar topics or reviews
- 📈 Interactive time-series dashboards
- 🌐 Geo-based customer maps (Folium Maps)
- 🎢 Sankey diagrams for product flow
- 🧱 Heatmaps and bar plots for market basket results
- 🪪 Customer segments using RFM scatter plots


---

## Tech Stack
- Used React, D3 and Folium Library for Frontend
- Used python based Fast API based backend hosted locally and Database used: Clickhouse (available during the semester only)

---

