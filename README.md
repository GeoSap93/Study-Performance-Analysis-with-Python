# Study-Performance-Analysis-with-Python
--------------------------------------------------------------------------------
Source: https://www.kaggle.com/datasets/bhavikjikadara/student-study-performance
---------------------------------------------------------------------------------
The inspiration of this study is to understand the influence of the parents' background, test preparartion, race/ethnicity and quality of lunch has on students' performance.

This analysis was carried out by using Python to read and print the entire DataFrame, to explore data with the use of Pandas (printing the first or last rows, printing general information,slicing specific rows or columns). Also, cleaning data like emptying cells, replacing empty values, finding and removing duplicates and printing the new DataFrame was carried out by using Pandas library.

The table below shows all info about our file. Our file has 8 columns which are consisted of three numeric columns and the other five have string data.
The total amount of students participating in this research was 1000.

Data columns (total 8 columns):
    Column                       Non-Null Count  Dtype 

 0   gender                       1000 non-null   object
 1   race_ethnicity               1000 non-null   object
 2   parental_level_of_education  1000 non-null   object
 3   lunch                        1000 non-null   object
 4   test_preparation_course      1000 non-null   object
 5   math_score                   1000 non-null   int64 
 6   reading_score                1000 non-null   int64 
 7   writing_score                1000 non-null   int64 
dtypes: int64(3), object(5)

The data in all five string columns are splint into the following variables in brackets with the use of unique() function: gender ('female', 'male'), race_ethinicity ('group B' 'group C' 'group A' 'group D' 'group E'), parental level of education ("bachelor's degree" 'some college' "master's degree" "associate's degree" 'high school' 'some high school'), lunch ('standard' 'free/reduced'), 
test preparation score ('none' 'completed').

By using the groupby() and size() function, we can see the 51.8% participants are females and 48.2% are males. In terms of their race/ethnicity, 8.9% belong in group A, 19% in group B, 31.9% in group C, 
26.2% in group D and 14% in group E. Based on the parental education level, 22.2% have a associate's degree, 11.8% have a bachelor's degree, 19.6% have a high school degree, 5.9% a master's degree, 22.6% did some college and the rest 17.9% did some high school. On their lunch size, 35.5% had a free/reduced lunch and the rest 64.5% had a standard lunch. Last, only 35.8% of the participants did prepared for the tests while the other 64.2% did no preparation.

During the analysis was carried our correlations between numeric columns (maths, reading and writing scores).

                Correlations	(Function: correl())
                Maths vs Reading	0.818
                Maths vs Writing	0.803
                Reading vs Writing	0.955

The outcome showed that there is a good and positive correlation between all scores which means that we can predict that the higher their maths score the higher their score will be in reading or writing. Also, we can see that there is a good and positive correlation (close to a perfect correlation) between reading and writing so we can predict that the higher their score is in reading the higher their writing score will be.  

