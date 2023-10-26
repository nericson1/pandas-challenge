# pandas-challenge

## Description: PyCity Schools Analysis
The first markdown cell of `PyCitySchools.ipnyb` contains a brief summary of the purpose of this data analysis, along with 3 key conclusions drawn from the calculations performed and DataFrames generated.

## References
### String Replacement
In the section titled 'Scores by School Spening' I found that I needed to change the 'Per Student Budget' value to a float from a string because I was getting errors when attempting to run the pd.cut() calculations to create the school_spending_df DataFrame. I could not turn the 'Per Student Budget' string into a float without first replacing the dollar sign with an empty string. I received a warning in Jupyter Notebook upon replacing the string using the str.replace method, and used the link copied below to determine that regex needs to be set equal to True in order for the string replacement to work. From there I could run .astype() to turn 'Per Student Budget' into a float.

link: https://pandas.pydata.org/docs/reference/api/pandas.Series.str.replace.html

### Index Name Removal
In the starter Jupyter notebook provided for us to use as an outline, I was introduced to the method of setting index.name equal to None which removes the index name from the given DataFrame. I used this method in the per_school_summary DataFrame (cell 19), the math_scores_by_grade DataFrame (cell 22), and reading_scores_by_grade DataFrame (cell 23) of the PyCitySchools jupyter notebook.
