# Study-Performance-Analysis-with-Python
--------------------------------------------------------------------------------
Source: https://www.kaggle.com/datasets/bhavikjikadara/student-study-performance
---------------------------------------------------------------------------------
The inspiration of this study is to understand the influence of the parents' background, test preparartion, race/ethnicity and quality of lunch has on students' performance.

This analysis was carried out by using Python to read and print the entire DataFrame, to explore data with the use of Pandas (printing the first or last rows, printing general information,slicing specific rows or columns). Also, cleaning data like emptying cells, replacing empty values, finding and removing duplicates and printing the new DataFrame was carried out by using Pandas library.

During the analysis was carried our correlations between numeric columns (maths, reading and writing scores) only with the use of excel.

                Correlations	(Function: correl())
                Maths vs Reading	0.818
                Maths vs Writing	0.803
                Reading vs Writing	0.955

The outcome showed that there is a good and positive correlation between all scores which means that we can predict that the higher the score students have in maths the higher their score will be in reading or writing. Also, we can see that there is a good and positive correlation (close to a perfect correlation) between reading and writing so we can predict that the higher their score is in reading the higher their writing score will be.  
