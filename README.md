Patient Segmentation Analysis

This project demonstrates a comprehensive workflow for segmenting patients using clustering techniques, with a focus on handling mixed data types and extracting actionable insights for healthcare decision-making.
This project was completed using Claude Code.

Project Overview:

The goal of this analysis was to segment a patient population based on demographic, clinical, and utilization features. The resulting clusters are intended to inform clinical and business strategies by identifying distinct patient segments.

Steps Followed:

1. Data Exploration
   
Explored the dataset to understand distributions, missing values, and correlations.

Assessed the need for preprocessing steps such as encoding categorical variables and scaling numerical features.

3. Data Preprocessing
   
Handled missing values appropriately.

Applied one-hot encoding to categorical variables for initial clustering attempts.

Scaled numerical features where necessary.

4. Model Selection & Tradeoffs

Initial Approach: Used K-Means clustering with one-hot encoded data.

Tradeoff: K-Means relies on Euclidean distance, which is not suitable for mixed data types (numerical + categorical). This led to poor cluster quality.

Improved Approach: Switched to clustering using Gower distance, which can handle mixed data types effectively.

Tradeoff: Gower distance is computationally more intensive but provides more meaningful clusters for heterogeneous data.

5. Clustering & Interpretation
   
Performed clustering using the appropriate distance metric.

Analyzed cluster characteristics to create narratives for each patient segment.

Visualized and interpreted the clusters to extract actionable insights.

6. Key Takeaways
   
Always explore your data first — distributions, missing values, and correlations tell you what preprocessing is needed.

AI-assisted coding accelerates the workflow but your domain knowledge is irreplaceable. You need to validate and sometimes correct the AI.

Algorithm choice matters: K-Means with one-hot encoding failed because Euclidean distance doesn't handle mixed data well. Gower distance was the right tool for this dataset.

Clustering is only useful if you can interpret it: the real value is in the patient segment narratives that inform clinical and business decisions.


Requirements
Python 3.x
pandas, numpy, scikit-learn, plotly, and other standard data science libraries

