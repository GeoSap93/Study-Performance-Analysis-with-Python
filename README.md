# Study-Performance-Analysis-with-Python
--------------------------------------------------------------------------------
Source: https://www.kaggle.com/datasets/bhavikjikadara/student-study-performance
---------------------------------------------------------------------------------
The aim of this study is to examine the impact of parental background, test preparation, race/ethnicity, and lunch quality on student performance.

This analysis was conducted using Python to access and display the entire DataFrame, utilizing Pandas to explore the data (such as printing the first or last rows, displaying general information, and slicing specific rows or columns). Additionally, data cleaning tasks such as removing empty cells, replacing missing values, identifying and eliminating duplicates, and displaying the updated DataFrame were performed using the Pandas library.

The table produced by using the function .info(), provides better insights on our file. It comprises 8 columns from which three are numeric and the rest five string. 
A total of 1000 students participated in this research.
Maths, Literacy and Reading Scores consist of our three numeric columns.

The data in all five string columns are split into the following variables within brackets using the unique() function: 
- Gender ('female', 'male')
- Race/ethnicity ('group B', 'group C', 'group A', 'group D', 'group E')
- Parental level of education ("bachelor's degree", 'some college', "master's degree", "associate's degree", 'high school', 'some high school')
- Lunch ('standard', 'free/reduced')
- Test preparation score ('none', 'completed')

Through the utilization of the groupby() and size() functions, it is observed that 51.8% of participants identify as female, while 48.2% identify as male. When examining race/ethnicity, the breakdown is as follows: 8.9% in group A, 19% in group B, 31.9% in group C, 26.2% in group D, and 14% in group E. Parental education levels are as follows: associate's degree (22.2%), bachelor's degree (11.8%), high school degree (19.6%), master's degree (5.9%), some college (22.6%), and some high school (17.9%). In terms of lunch types, 35.5% received free/reduced lunch, while 64.5% had a standard lunch. It is notable that only 35.8% of participants prepared for the tests, with the remaining 64.2% reporting no preparation.

During the analysis, correlations between numeric columns (maths, reading and writing scores) were carried out.

                Correlations	(Function: correl())
                Maths vs Reading	0.818
                Maths vs Writing	0.803
                Reading vs Writing	0.955

The results indicate a strong and positive correlation among all scores, suggesting that higher scores in math is associated with higher scores in reading and writing. Furthermore, there is a high correlation between reading and writing scores, implying that higher reading scores are likely to correspond with higher writing scores.
