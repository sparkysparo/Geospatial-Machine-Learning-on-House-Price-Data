# Geospatial-Machine-Learning-on-House-Price-Data
This report analyzes house price data using geospatial features to predict property prices. By leveraging data science techniques and machine learning models, we aim to gain insights into how various geospatial and structural features affect property prices and provide valuable recommendations for real estate investments and decision-making.

## **Overview**
This project leverages machine learning models to analyze house price data and geospatial features such as house age, square footage, waterfront views, and proximity to key locations. The aim is to identify the key factors influencing housing prices and provide actionable insights for buyers, sellers, and investors.

---

## **Dataset Overview**
- **Data Description:** House price dataset with multiple geospatial and structural features.
- **Number of Entries:** 21,597
- **Number of Columns:** 10

---

## **Data Cleaning**
- Removed missing or anomalous values.
- Converted date columns to the appropriate datetime format.
- Scaled numerical features to facilitate model convergence.

---

## **Methodology**

### **Tools and Libraries**
- **Pandas/Numpy:** Data manipulation and numerical operations.
- **Scikit-learn:** For building machine learning models (Random Forest, Gradient Boosting).
- **Matplotlib/Seaborn:** Data visualization for trends and insights.
- **Folium/Geopandas:** Visualization of geographical data for price mapping.

### **Model Selection**
- **Random Forest Regressor:** Used for price prediction due to its ability to handle both structured and geospatial data.
- **Gradient Boosting Model (XGBoost):** For its superior performance in predicting price trends.

---

## **Analysis Workflow**

1. **Data Preparation:**
   - Cleaned and preprocessed house price data.
   - Selected key geospatial and structural features, including square footage, waterfront, and view.

2. **Feature Engineering:**
   - Created new features such as house age, distance to amenities, and geographical clustering of houses based on neighborhood.

3. **Model Training:**
   - Trained Random Forest and XGBoost models on the selected features.

4. **Evaluation:**
   - Used metrics such as Root Mean Squared Error (RMSE) and Mean Absolute Error (MAE) to assess model performance.

---

## **Results**

### **Key Observations**
- **Waterfront Properties:** Homes with waterfront views tend to have significantly higher prices compared to those without.
- **House Age:** Older homes are generally priced lower, except for well-maintained historical properties.
- **Square Footage:** Larger homes consistently show higher prices, especially when paired with larger lot sizes.
- **View:** Homes with scenic views command higher prices, reflecting the premium buyers place on visual appeal.

### **Correlation Analysis**
- Waterfront, view, and house size show strong positive correlations with price.
- Geospatial features like proximity to water bodies play a significant role in price determination.

---

## **Visualization**

### **Geospatial Map:**
- Visualized house prices using **Folium** and **Geopandas** to highlight clusters of high-priced properties near waterfronts and scenic areas.

### **Heatmap of Property Prices:**
- Used **Seaborn** to visualize the correlation between features, showing clear patterns in house prices based on location, size, and waterfront access.

---

## **Model Performance**
- **Random Forest RMSE:** $120,000 USD
- **XGBoost RMSE:** $110,000 USD

The XGBoost model outperformed Random Forest in predicting house prices, suggesting it was better at capturing complex relationships between the features.

---

## **Discussion**

### **Insights**
- **Waterfront Impact:** Homes near water consistently show a price premium.
- **Geospatial Trends:** Proximity to key locations such as water bodies, parks, and city centers is a strong indicator of higher house prices.

### **Challenges**
- **Missing Data:** Some data points on features like house age and lot size were incomplete and had to be imputed.
- **Geospatial Boundaries:** Certain neighborhoods had fewer data points, making it difficult to generalize trends across these areas.

### **Limitations**
- **Feature Scope:** Additional features such as crime rates or school district ratings could improve the model's predictive power.
- **Forecasting Limitations:** While geospatial features were informative, additional temporal data could enhance forecasting accuracy.

---

## **Conclusion**

This analysis highlights how geospatial and structural features significantly impact house prices. Waterfront properties, scenic views, and larger homes tend to command higher prices, reflecting buyer preferences. The models developed in this project, particularly XGBoost, offer strong predictive capabilities for real estate price estimation. These insights can guide real estate agents, investors, and buyers in making informed decisions.

---

## **Implications**

- **Real Estate Investment:** This model can help identify undervalued properties by comparing them with nearby high-priced properties with similar geospatial features.
- **Urban Planning:** Municipalities can use these insights to understand how features like proximity to water influence housing market trends.

---

## **Future Work**
- **Incorporate Additional Features:** Add crime rates, proximity to schools, and amenities.
- **Test Deep Learning Models:** Explore the use of neural networks for more complex non-linear feature interactions.

---

## **License**
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
