# Performance-Analysis-of-R-and-Python

![alt text](https://github.com/Nirvi1/Performance-Analysis-of-R-and-Python/blob/master/Performance_Analysis_R_Python.PNG)

Comparison of R and python with 29MB data , having 550 accounts and 906 entities-


# Input
Reading 75MB file with 57922 columns, 70 rows 2 times each having 2 different frames. Combined it will be 150MB data.


# Reading Input Dataset

Instead of getting file contents all at once, I am reading specific rows from the file i.e reading columns and rows for one frame first then for other frame.
Time taken to read , process , filter data in R : 12 seconds 
Time taken to read , process , filter data in Python : 25 seconds 

#Conclusion based these two experiments
•	Filtering data is more fast in R than python. 
•	Reading data is faster in python if reading complete file.
•	With 75+75MB =150MB it takes 0.09 seconds to filter columns  than in python that takes 0.35 seconds 
•	It takes 11 seconds to read when getting only specific rows, and process 150MB data in R vs in Python which takes 24 seconds to do the same. So R is faster in this case than python.


