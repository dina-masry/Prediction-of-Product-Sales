![Data science](https://github.com/user-attachments/assets/35c8d9c8-c0b0-4f7a-badf-cb9b4caba0f5)

# Sale Prediction for Food Items: A Data Science Project
This data science project focuses on developing a robust and accurate model for predicting sales of food items. By leveraging historical sales data, item characteristics, and potentially external factors, the project aims to provide valuable insights for businesses in the food industry.
Following the data cleaning and exploratory data analysis (EDA) phase, this project has generated insightful visualizations to understand the underlying patterns in food item sales.

## The EDA process involved:

### Data Cleaning: 
  Addressing missing values, remove duplicates , and ensuring data consistency across various features.
### Visual Exploration: 
  Creating a range of plots (e.g., histograms, scatter plots, box plots, heatmap) to examine the distribution of sales, relationships between variables, and temporal 
  trends.
  - Histogram and boxplot for Item_visibility :
    
    ![Item_visiability graphs](https://github.com/user-attachments/assets/33769550-3adc-475c-ac99-dd3110bd8f7a)
     - This histogram shows that Item_visibilty values is the most frequency is less than 1
     - Boxplot shows than:
         -min is 0
         -max is nearby 0.33
         -median is nearby 0.06
         -Q1 is nearby 0.03
         -Q3 is nearby 0.9
        -There are lots of outliers
        -It seems to be right skewed
  - Histogram and boxplot for Item_weight :
    
    ![Item_weight graphs](https://github.com/user-attachments/assets/7b1ce083-c66c-4078-821c-78830aa0ca51)
    - Histogram shows that Item weights between 12.5 and 13.5 have the most frequency count ~=1600 and differ alot from the other values which their counts are 
      less than 500.
    -Boxplot shows 
       - min is nearby 4.5 
       - max is nearby 21
       - Q1 is nearby 9 
       - Median is nearby 13
       - Q3 is nearby 16
       - There is no any outliers
       - Graph seems to be left skewed
  - Countplot for outlet_identifier :
    
    ![outlet_identifier bar plot](https://github.com/user-attachments/assets/16b971fe-7b9b-4a48-8a3e-53208b46e7e9)
    - This countplot shows that all outlet_identifier have the same count(approximetly) expect OUT010 AND OUT019.
  - Countplot for outlet_size:
    
    ![oulet_size count plot](https://github.com/user-attachments/assets/c0a46551-5ba5-4579-8a07-7bf6e8836ff1)
    - This countplot shows that medium has the highest count while high has the lowest.
  - Heatmap:
    
    ![Heatmap for food sales](https://github.com/user-attachments/assets/4dcd8692-d584-4a25-b3cc-7995b7f524c8)
    - Heatmap shows that there is no any strong correlations.
    - There is a moderate positive correlation between Item_MRP and Item_outlet_Sales.

## Model: Linear regression
  This project employs Linear Regression to develop a predictive model for food item sales. We selected this model for its strong balance of:
   - Transparency: Coefficients reveal the direct impact of features like price, promotional activities, and seasonal trends on sales, offering clear business   insights.
   - Efficiency: It's a computationally light model, ideal for rapid prototyping and establishing a foundational understanding of sales drivers.
   - Baseline Performance: Linear Regression provides a robust benchmark against which the performance of more sophisticated models can be measured.
   Our goal is to leverage these linear relationships to build an insightful and effective sales forecasting tool.
  Its evaluation mertics:
Regression Metrics: Training Data
 - MAE = 847.129
 - MSE = 1,297,558.136
 - RMSE = 1,139.104
 - R^2 = 0.562
--------------------------------------------------------------------------------------------------
Regression Metrics: Test Data
  - MAE = 804.120
  - MSE = 1,194,349.715
  - RMSE = 1,092.863
  - R^2 = 0.567




## Key observations from the visualizations include:
- Sales Distribution: Understanding the spread and central tendency of sales figures across different food items and time periods.
- Feature Relationships: Identifying potential correlations between item characteristics (e.g., category, MRP, outlet size) and sales performance.
- Outlier Identification: Visualizing extreme sales values that might require further investigation or specific handling during the modeling phase.
These visual insights form a strong foundation for the subsequent steps in the project, particularly feature engineering and model selection. The observed patterns and relationships will guide the creation of relevant features and the choice of appropriate predictive models to accurately forecast food item sales.
