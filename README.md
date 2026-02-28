Exploratory Data Analysis
_____________________________________________________________________________________________________________________________________________________________________
This repository contains the work for exploring 2 datasets. Two datasets are explored through statistical summaries, correlation analysis, and visualizations.
_____________________________________________________________________________________________________________________________________________________________________
Repository Contents                            File	Description
1. PDS_Assignment_1.ipynb  ---	Main Jupyter notebook containing all analysis code
2. StudentsPerformance.csv	--- Student exam scores dataset
3. frailty_data.csv	        --- Frailty and physical measurements dataset
4. findings.md	           --- Summary statistics and correlation findings for the frailty dataset
5. V1_Gender_Boxplots.png  --- Math & Reading scores distribution by gender
6. V2_TestPrep_Math.png	   --- Math score distribution by test preparation course
7. V3_Lunch_Performance.png	--- Average overall score by lunch type
8. V4_Correlation_Heatmap.png --- Correlation heatmap across all three exam subjects
9. V5_Scatter_Trend_Enhanced.png --- Math vs. Reading score scatter plot by test prep status
_____________________________________________________________________________________________________________________________________________________________________

Datasets
1. Students Performance (StudentsPerformance.csv)
Contains exam scores for 1,000 students across three subjects (math, reading, writing), along with demographic and background factors including gender, lunch type, and test preparation course completion.
2. Frailty Data (frailty_data.csv)
Contains physical measurements for 20 individuals including height, weight, age, grip strength, and a binary frailty classification. Derived features (BMI, metric units) were computed during analysis.
_____________________________________________________________________________________________________________________________________________________________________

Key Findings
1. Students Performance
•	Gender: Female students tend to score higher in reading and writing, while male students score slightly higher in math. Both groups show similar overall distributions (V1).
•	Test Preparation: Students who completed a test prep course scored notably higher in math, with a higher median and tighter IQR compared to those with no preparation (V2).
•	Lunch Type: Students with a standard lunch plan averaged ~71 overall, versus ~62 for those on free/reduced lunch a meaningful gap suggesting socioeconomic influence on performance (V3).
•	Subject Correlations: All three subjects are highly correlated. Reading and writing share the strongest relationship (r = 0.95), while math correlates at 0.82 with reading and 0.80 with writing (V4).
•	Math vs. Reading by Test Prep: A strong positive linear trend exists between math and reading scores for both groups (R² ≈ 0.63–0.67). Students who completed test prep cluster toward higher scores (V5).

2. Frailty Data
•	Summary Statistics: Mean BMI was 19.68 (lean range), mean age was 32.5 years, and 40% of individuals were classified as frail.
•	Grip Strength & Frailty: A moderate negative correlation of r = –0.476 was found between grip strength and frailty classification, indicating that lower grip strength is associated with higher likelihood of frailty.
_____________________________________________________________________________________________________________________________________________________________________

How to Run
1.	Clone this repository or download the files.
2.	Install dependencies: 
3.	pip install pandas numpy matplotlib seaborn jupyter
4.	Launch the notebook: 
5.	jupyter notebook PDS_Assignment_1.ipynb
6.	Run all cells in order to reproduce all statistics and visualizations.
_____________________________________________________________________________________________________________________________________________________________________

Requirements

•	Python 3.8+
•	pandas
•	numpy
•	matplotlib
•	seaborn
•	jupyter

