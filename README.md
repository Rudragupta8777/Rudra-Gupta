# EDA Course Project

**Name:** Rudra Gupta  
**Registration Number:** 23BDS0306  
**Institution:** Vellore Institute of Technology (VIT)  

## Project Overview
This repository contains the code and documentation for the EDA Course Project. It includes the step-by-step implementation of Exploratory Data Analysis on the provided `horse.csv` dataset, utilizing data science techniques such as data cleaning, transformation and advanced statistical visualizations.

## Libraries Used
* `pandas` & `numpy`: Data manipulation and numerical calculations.
* `matplotlib.pyplot`, `mpl_toolkits.mplot3d` & `seaborn`: 2D and 3D data visualization.
* `scipy.stats` & `scipy.cluster.hierarchy`: Advanced statistical calculations and hierarchical dendrograms.
* `sklearn.preprocessing` & `sklearn.cluster`: Data transformation, label encoding, K-Means, and Agglomerative clustering.

---

## Phase 1: Data Preprocessing and Initial EDA

The objective of this phase is to prepare the raw dataset for analysis by systematically handling missing values and outliers, followed by uncovering foundational data patterns through statistical summaries and visualizations.

### Tasks Completed in Phase 1
1. **Loading the Dataset:** 
   Imported the `horse.csv` dataset and initialized the Python environment.
2. **Basic Statistical Analysis:** 
   Generated statistical summaries (`.describe()`) and inspected the dataset's structure, data types, and initial records.
3. **Handling Missing Data:** 
   - Identified missing values across all columns.
   - Dropped columns containing more than 70% missing data.
   - Imputed missing numerical values using the `mean`.
   - Imputed missing categorical values using the `mode`.
4. **Data Cleaning:** 
   Removed duplicate rows, standardized all text data to lowercase, and converted character variables into categorical data types.
5. **Data Transformation:** 
   - Utilized `LabelEncoder` to convert the `outcome` and `surgery` categories into numerical formats for correlation analysis.
   - Identified and removed extreme outliers in the `pulse` column using the Interquartile Range (IQR) method.
6. **Univariate Analysis:** 
   Created a histogram with a KDE curve, a percentage bar chart, and a violin plot to analyze individual variables like pulse, outcome, and rectal temperature.
7. **Bivariate Analysis:** 
   Explored relationships between two variables using a scatter plot (rectal temp vs. pulse), a boxplot (pulse across outcomes), and a bar chart (average pulse by surgery status).
8. **Multivariate Analysis:** 
   Visualized complex relationships using a correlation heatmap, a FacetGrid (pulse distribution by outcome), and a 4-variable scatter plot colored by outcome and sized by packed cell volume.

---

## Phase 2: Statistical Analysis & Clustering

The objective of this phase is to execute comprehensive 1D, 2D, 3D, and multi-dimensional statistical analyses, followed by unsupervised machine learning techniques to identify inherent groupings within the dataset.

### Tasks Completed in Phase 2
1. **1D Statistical Analysis:** 
   Computed a complete suite of summary statistics (mean, variance, skewness, kurtosis) into a structured DataFrame. Visualized numerical and categorical distributions using pie charts, bar plots, binned histograms, and box plots.
2. **2D Statistical Analysis:** 
   Constructed contingency tables with proportional distribution calculations. Grouped numerical data by category to calculate segmented statistics, visualizing the relationships via grouped violin plots and stacked bar charts. Modeled continuous variable relationships using Pearson/Spearman coefficients and linear regression trendlines.
3. **3D Statistical Analysis:** 
   Constructed a 3D scatter plot utilizing `mpl_toolkits.mplot3d` to visualize the simultaneous spatial relationship between Rectal Temperature, Pulse, and Packed Cell Volume.
4. **Multivariate (ND) Analysis:** 
   Generated faceted box plots and error-bar grouped charts to analyze statistics across multiple categorical intersections. Mapped full numeric correlations via heatmaps and `seaborn.pairplot` matrices.
5. **K-Means Clustering:** 
   Standardized numerical subsets and applied K-Means algorithms. Iterated Within-Cluster Sum of Squares (WCSS) for K from 1 to 10 to generate an Elbow Plot, allowing for optimized centroid selection.
6. **Hierarchical Clustering:** 
   Calculated Euclidean distance matrices to map hierarchical aggregations. Generated and compared dendrograms utilizing Single, Complete, and Ward linkage methods. Cut the final hierarchy into 3 discrete clusters and tabulated sample assignments.

---
