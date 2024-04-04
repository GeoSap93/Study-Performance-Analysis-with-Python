# Study-Performance-Analysis-with-Python
--------------------------------------------------------------------------------
Source: https://www.kaggle.com/datasets/bhavikjikadara/student-study-performance
---------------------------------------------------------------------------------
The inspiration of this study is to understand the influence of the parents' background, test preparartion, race/ethnicity and quality of lunch has on students' performance.

This analysis was carried out by using Python to read and print the entire DataFrame, to explore data with the use of Pandas (printing the first or last rows, printing general information,slicing specific rows or columns). Also, cleaning data like emptying cells, replacing empty values, finding and removing duplicates and printing the new DataFrame was carried out by using Pandas library.

The table below shows all info about our file. Our file has 8 columns which is consisted if three numeric columns and the other 5 have string data.
The total amount od students participating in this research was 1000.

Data columns (total 8 columns):
 #   Column                       Non-Null Count  Dtype 
---  ------                       --------------  ----- 
 0   gender                       1000 non-null   object
 1   race_ethnicity               1000 non-null   object
 2   parental_level_of_education  1000 non-null   object
 3   lunch                        1000 non-null   object
 4   test_preparation_course      1000 non-null   object
 5   math_score                   1000 non-null   int64 
 6   reading_score                1000 non-null   int64 
 7   writing_score                1000 non-null   int64 
dtypes: int64(3), object(5)

The data in all five string columns are splint into the following variables: 

Gender: ['female' 'male']
Race_ethnicity: ['group B' 'group C' 'group A' 'group D' 'group E']
Parental_level_of_education: ["bachelor's degree" 'some college' "master's degree" "associate's degree" 'high school' 'some high school']
Lunch: ['standard' 'free/reduced']
Test_preparation_score: ['none' 'completed']

The folowing tables show the size of the group based on the string data:

 gender  size
0  female   518
1    male   482

In this research, took part 518 female students and 482 male students.

race_ethnicity  size
0        group A    89
1        group B   190
2        group C   319
3        group D   262
4        group E   140

Between the race/ethinicity groups, the group C had most participants and the group A had the least. 

parental_level_of_education  size
0          associate's degree   222
1           bachelor's degree   118
2                 high school   196
3             master's degree    59
4                some college   226
5            some high school   179

On the parental level of education, we had only 59 with a master degree and 118 with a bachelor. 

   lunch  size
0  free/reduced   355
1      standard   645

In terms of the lunch size, most of the students had a standard lunch.

test_preparation_course  size
0               completed   358
1                    none   642

A persentage of 64.2% had no preparation for the tests and the rest 35.8% were prepared.

During the analysis was carried our correlations between numeric columns (maths, reading and writing scores) only with the use of excel.

                Correlations	(Function: correl())
                Maths vs Reading	0.818
                Maths vs Writing	0.803
                Reading vs Writing	0.955

The outcome showed that there is a good and positive correlation between all scores which means that we can predict that the higher the score students have in maths the higher their score will be in reading or writing. Also, we can see that there is a good and positive correlation (close to a perfect correlation) between reading and writing so we can predict that the higher their score is in reading the higher their writing score will be.  

