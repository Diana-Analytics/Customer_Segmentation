# Customer Segmentation Using K-Means Clustering
### Overview

This project applies K-Means clustering to segment customers based on their purchasing behavior. The goal is to identify distinct customer groups, helping businesses tailor their marketing strategies and improve customer engagement.
### Dataset

The dataset contains customer information such as year_birth, marital_status, education_status, annual income, recency, etc.

Source: The dataset is from Kaggle

### **Libraries Used**  
- `pandas` – Data manipulation  
- `numpy` – Numerical operations  
- `matplotlib` / `seaborn` – Data visualization  
- `scikit-learn` – Machine learning (K-Means, PCA, scaling, etc.)  
- `yellowbrick` – **KElbowVisualizer** for optimal K selection  

## **Project Steps**

 ### Data Cleaning & Preprocessing
  - Handled missing data.
  - Checked for duplicates (none found).
  -  Encoded categorical data using Label Encoding.
  -  Scaled numerical features for better clustering performance.

 ### Feature Engineering
  Created new features to enhance clustering effectiveness:
  - Age Groups – Categorized customers based on age.
  - Spending Ratio – Ratio of total spending to recency.
  - Family Size – Derived from total people in a household.
  - Total Spent – Aggregated spending across products.

### Exploratory Data Analysis (EDA)
- Analyzed frequency distribution of relevant columns using subplots for better visualization.
- Identified outliers using a boxplot, focusing on the Age column.
- Used IQR method to detect outliers and applied Winsorization to cap extreme values.

### Choosing the Optimal Number of Clusters (K)
- Applied the Elbow Method to determine the best number of clusters.

### Dimensionality Reduction & Visualization
- Used PCA (Principal Component Analysis) to reduce data to 2D for visualization.
- Plotted a scatter plot to visualize the clusters.

### Cluster Profiling & Insights
- Analyzed the characteristics of each cluster.
- Interpreted behavioral patterns within each segment.
- Drew conclusions on how the clusters can be used for targeted marketing or customer engagement strategies.

## **Results & Findings**  
After applying **K-Means clustering**, we identified **five distinct customer segments**:  

| **Cluster** | **Segment Name**                 | **Characteristics** |
|------------|----------------------------------|----------------------|
| **0**      | Young Low-Income Families       | Younger customers with lower income, likely early in their careers, balancing expenses for family needs. |
| **1**      | Affluent Empty Nesters          | High-income individuals, typically older, with fewer financial dependents, allowing for discretionary spending. |
| **2**      | Wealthy Seniors, Less Active    | Senior customers with significant wealth but lower spending activity, possibly saving more than spending. |
| **3**      | Middle-Class Large Families     | Households with moderate income, managing larger families, likely focused on budget-conscious purchases. |
| **4**      | Older Frequent Shoppers         | Older customers with consistent spending habits, possibly loyal shoppers with routine purchasing behavior. |

## **Recommendations (Cluster-Specific Approach)**  

Based on the identified customer segments, businesses can optimize their strategies as follows:  

| **Cluster** | **Suggested Strategy** |
|------------|------------------------|
| **Young Low-Income Families** | Offer **budget-friendly products**, discounts, and installment plans to support affordability. Partner with financial services for small credit options. |
| **Affluent Empty Nesters** | Promote **luxury & premium services**, exclusive memberships, and high-end experiences. Highlight convenience and exclusivity. |
| **Wealthy Seniors, Less Active** | Focus on **health & retirement-related services**, personalized assistance, and high-value investments. Consider home delivery and concierge services. |
| **Middle-Class Large Families** | Provide **family bundles, cashback rewards**, and special deals on bulk purchases. Offer financial planning tools for managing expenses. |
| **Older Frequent Shoppers** | Enhance **loyalty programs, special perks**, and personalized offers based on purchase history. Introduce VIP shopping experiences. |

## **Conclusion**  

This customer segmentation analysis using **K-Means clustering** provided valuable insights into different consumer groups, allowing businesses to **personalize their marketing, pricing, and service strategies**.  

By understanding the unique characteristics of each segment, companies can:  
✅ Improve customer experience through **targeted promotions**  
✅ Optimize pricing & product offerings based on **spending habits**  
✅ Increase **customer retention** with loyalty programs tailored to each group  

With these actionable insights, businesses can **maximize revenue, enhance customer satisfaction, and stay competitive** in the market. 🚀  


