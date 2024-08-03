# Segmenting Customers based on Income and Feedback
Understanding customer behavior is crucial for businesses to tailor their strategies effectively. This analysis focuses on segmenting customers based on two key factors: income and feedback. By applying K-Means clustering to a dataset containing customer income and feedback information, we aim to identify distinct customer groups. These segments can provide valuable insights for targeted marketing, product development, and customer retention initiatives.

## Data Preparation
### Import
This initial step involves gathering the necessary tools for the analysis. We import essential Python libraries such as <code>Pandas</code> for data manipulation, <code>NumPy</code> for numerical operations, and <code>Matplotlib</code>  and <code>Seaborn</code>for data visualization and some modules from<code>Sklearn</code> for model buiding. Additionally, we load the retail customer dataset, which contains information about customer income and feedback, into our environment. These components form the foundation for the subsequent data exploration and modeling processes.
### Explore
The goal is to ensure data integrity and consistency. A comprehensive exploratory data analysis (EDA) was conducted to understand the distribution, relationships, and potential outliers within the dataset. While numerous steps were undertaken, including statistical summaries, visualizations, and correlation analysis, this section presents a condensed overview due to space constraints. 

The original dataset is split into two based on the mask: rows with missing "Transaction_ID" and rows with complete data. Duplicate rows within the complete data subset are removed based on the "Transaction_ID" column, keeping the first occurrence. The cleaned dataset without duplicates and the dataset with missing "Transaction_ID" are combined into a new dataframe, resulting in a dataset with 294,795 rows and 30 columns.
### Split
The relevant columns "Income" and "Feedback" are extracted from the dataset. The <code>SimpleImputer</code> is used to replace missing values with the most frequent value for each column. These two categorical features are then converted into numerical representations using <code>OneHotEncoder</code>. The final preprocessed data, ready for the clustering model, is assigned to the variable <code>X</code>.

## Build Model
This section outlines the construction and training of the K-Means clustering model. Please refer the file **Segmenting Customers Based on Income and Feedback.ipynb** available in this repository to see how the model was build.
### Iterate
The optimal number of clusters was determined through model tuning using <code>silhouette_score</code> and <code>inertia_errors</code>.
## Communicate Results
<img width="1338" alt="Screenshot 2024-08-02 at 4 55 32 PM" src="https://github.com/user-attachments/assets/11e04a2a-d23d-4d8f-90a7-e71e80fe0f78">
A visual representation of the clusters, captured from the Notebook.

#### Key Observations

1. **Cluster 0**: This cluster has the highest mean income (Income_High) and a relatively high mean feedback (Feedback_Excellent). It can be interpreted as a group of high-income customers with excellent feedback.
2. **Cluster 1**: This cluster shows a mixed picture. While the income is moderate (Income_Medium), the feedback is quite diverse, ranging from bad to excellent. This cluster might represent a group of customers with varying income levels and diverse opinions about the product/service.
3. **Cluster 2**: This cluster has the lowest mean income (Income_Low) and a relatively low mean feedback (Feedback_Bad). It can be interpreted as a group of low-income customers with generally negative feedback.

**Further Insights and Actions**

* **Target Marketing**: Cluster 0 represents a valuable segment of high-income customers with positive feedback. Targeted marketing campaigns focusing on premium products or services could be effective for this group.
* **Customer Satisfaction**: Cluster 2, with low income and negative feedback, requires attention. Analyzing the reasons for negative feedback and implementing measures to improve customer satisfaction could be crucial.
*  **Product/Service Improvement**: Understanding the diverse feedback in Cluster 1 can provide insights into product/service improvements to cater to a wider customer base.

The results presented here provide a preliminary understanding of customer segments based on income and feedback. To gain deeper insights and enhance the model's predictive power, incorporating additional customer attributes.
