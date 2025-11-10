# Data-Science-Task---1
Healthcare Dataset Analysis: Distribution Visualization (Task 1)
This repository contains the initial data exploration and visualization for a healthcare dataset, focusing on visualizing the distribution of key variables as part of Task 1.
The primary goal of this task was to create appropriate charts (histograms and bar charts) to visualize the distribution of both a continuous variable (Age) and a categorical variable (Blood Type).

# Setup and Data
The analysis was performed using Python libraries pandas, matplotlib.pyplot, and seaborn.
Dataset: healthcare_dataset.csv
Total Entries: 55,500 records.
Key Columns Analyzed: Age (Continuous, int64) and Blood Type (Categorical, object).
Data Quality: No missing values (NaN) were found across any of the 15 columns, including the key variables Age and Blood Type.

# Visualizations
1. Age Distribution (Histogram)
A histogram was used to visualize the distribution of patient ages.
Chart Type: Histogram with a Kernel Density Estimate (KDE) curve.
Observation: The distribution of ages appears relatively uniform across the range of approximately 18 to 85, with a gentle curve, indicating a broad representation of age groups in the dataset.

Code Snippet:
Python
sns.histplot(df['Age'], bins=20, kde=True, color='green')
plt.title('Age Distribution of Patients')
(See Age Distribution of Patients chart on page 3)

2. Blood Type Distribution (Bar Chart/Countplot)
A countplot (bar chart) was used to show the frequency of different blood types.
Chart Type: Bar Chart/Countplot.
Observation: The count of patients for each of the eight blood types (B-, A+, A-, O+, AB+, AB-, B+, O-) is remarkably even, hovering around 7,000 counts per type.

Code Snippet:
Python
sns.countplot(x='Blood Type', data=df)
plt.title('Blood Type Distribution')
(See Blood Type Distribution chart on page 4)
