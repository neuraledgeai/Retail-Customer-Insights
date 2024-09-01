# Segmenting Customers based on Income and Feedback
Understanding customer behavior is crucial for businesses to tailor their strategies effectively. The aim of this analysis is to segment customers based on income levels and their corresponding feedback patterns to identify opportunities for enhancing customer satisfaction and driving business growth.

>[!TIP]
>For a deeper dive into the data and methods used in this project, please check out the <code>Retail_Cluster_Analysis.ipynb</code>[^1] notebook. Whether you're interested in the technical details or the insights derived from the analysis, the notebook provides a comprehensive overview of the entire project.
[^1]: You can download the <code>Retail_Cluster_Analysis.ipynb</code> notebook directly from this repository and run it in your own Jupyter Lab environment. This allows you to explore the data, modify the analysis, and see the results firsthand.

## Communicate Results
<img width="1338" alt="Screenshot 2024-08-31 at 3 16 59 PM" src="https://github.com/user-attachments/assets/6a08996b-9e3f-49bb-a60c-4861c80f7b27">
A visual representation of the clusters, captured from the Notebook.

### Interpretation

**Cluster 0**

- **Income_Medium** is the dominant group with a value of 1, meaning that this cluster consists entirely of medium-income individuals.
- Among the feedback categories, **Feedback_Excellent** has the highest value at 0.48, indicating that nearly half of the feedback from this group is excellent.
- **Feedback_Average** has a value of 0.3, which suggests that a significant portion, though not the majority, of this cluster's feedback is average.
- **Feedback_Bad** has a value of 0.22, indicating that a smaller, yet notable portion of this cluster gave negative feedback.

**Cluster 1**

- **Income_Low** is the predominant income group with a value of 0.7, while **Income_Medium** also appears with a value of 0.3, indicating a mix of low and medium-income individuals in this cluster.
- **Feedback_Good** has the highest value at 0.53, suggesting that the majority of feedback from this cluster is positive.
- **Feedback_Excellent** has a value of 0.25, indicating a significant portion of high satisfaction.
- **Feedback_Average** and **Feedback_Bad** have smaller values of 0.13 and 0.08, respectively, showing that a minority of individuals in this cluster provide average or bad feedback.

**Cluster 2**

- **Income_High** dominates this cluster with a value of 1, meaning this cluster is composed entirely of high-income individuals.
- Feedback in this cluster is spread fairly evenly across categories, with **Feedback_Excellent** at 0.31 and **Feedback_Good** at 0.3, indicating that high-income individuals in this cluster tend to give positive feedback.
- **Feedback_Average** and **Feedback_Bad** have values of 0.23 and 0.16, respectively, showing some degree of less-than-positive feedback within this high-income group.

### Implications

**1. Cluster 0: Medium-Income Group**

**Profile**: This cluster consists entirely of medium-income individuals.

**Feedback Breakdown**:

- 48% give excellent feedback.
- 30% give average feedback.
- 22% give bad feedback.

**Actionable Insights**

- **Focus on retention strategies**: Since nearly half of this group provides excellent feedback, these customers are likely satisfied and loyal. Implement loyalty programs or special offers to maintain their satisfaction and encourage repeat business.
- **Address the 22% who are dissatisfied**: A notable portion gives bad feedback, indicating underlying issues. Conduct further research to understand the specific pain points and address them through improved customer service, product adjustments, or targeted communication.

**1. Cluster 1: Low and Medium-Income Group**

**Profile**: This cluster primarily consists of low-income individuals (70%) with a significant portion of medium-income individuals (30%).

**Feedback Breakdown**:

- 53% give good feedback.
- 25% give excellent feedback.
- 13% give average feedback.
- 8% give bad feedback.

**Actionable Insights**

- **Enhance value propositions**: Since a majority give good feedback, emphasize value-for-money propositions in your marketing. Promotions or budget-friendly product bundles could further enhance satisfaction, particularly for the low-income segment.
- **Upsell opportunities for medium-income customers**: The 30% medium-income group could be open to more premium products or services. Tailor communications to highlight higher-value offerings, potentially increasing overall customer spend.
- **Continue monitoring the 8% who give bad feedback**: Although a small segment, consistently review their concerns to avoid escalation and maintain the overall positive trend.

**1. Cluster 2: High-Income Group**

**Profile**: This cluster consists entirely of high-income individuals.

**Feedback Breakdown**:

- 31% give excellent feedback.
- 30% give good feedback.
- 23% give average feedback.
- 16% give bad feedback.

**Actionable Insights**

- **Premium product offerings**: With a high proportion of good and excellent feedback, this group is likely interested in premium or exclusive products. Consider introducing luxury items, exclusive events, or personalized services to cater to their preferences.
- **Address dissatisfaction proactively**: The 16% giving bad feedback is relatively high for a high-income segment. Investigate the root causes—whether it’s service quality, product expectations, or other factors—and implement high-touch customer service strategies to resolve their issues.
- **Opportunities for improvement**: The 23% providing average feedback suggests there’s room to enhance the overall experience. Look into refining the customer journey for this segment to shift more individuals from average to good or excellent satisfaction levels.

### General Strategy

- **Segmentation-Based Marketing**: Tailor marketing strategies to each cluster based on their income levels and feedback tendencies. For example, loyalty programs for Cluster 0, value-focused promotions for Cluster 1, and premium offerings for Cluster 2.
- **Targeted Service Improvements**: Focus on improving the experience for those providing average or bad feedback across all clusters. This could involve refining customer service, better understanding their needs, or revisiting product features.
- **Data-Driven Decision-Making**: Regularly monitor the feedback trends within each cluster to adapt strategies dynamically, ensuring you remain responsive to customer needs and expectations.

The results presented here provide a preliminary understanding of customer segments based on income and feedback. And remember, these results are specific to the dataset and may not be generalizable to other contexts.
