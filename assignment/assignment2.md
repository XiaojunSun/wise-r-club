## Assignment 2

WISE R CLUB, Xiaojun Sun, 2014.07.11

This is the second assignment for WISE R Club members. You'd better read Chapter 5 to Chapter 8 of R in Action before trying to finish this assignment. The questions are described as following.

***************************

**CONTENTS**

[TOC]

-----------------------------

### Question 1
Write a factorial function with the name `Fac` by yourself. The function can realize the flowing features: $Fac(n)=1$ if $n=0$ and $Fac(n)=n(n-1)(n-2)...1$ for any integer $n>0$. Please not use the `factorial()` function provided in R, try to write your own factorial function. Make the function as simple and short as possible. 

### Question 2
Based on the dataset `grades.txt` which I gave you in the last assignment, answer the following questions. 

#### Question 2.1
Draw the box plots of the test scores of the three courses: `Math`, `Chinese` and `English` in one graph just like Figure 6.12 in the book.

#### Question 2.2
Take sum of the test scores of the three courses(Math, Chinese and English), record it as variable `Sum`. Grade each student from `A+` to `D` based on the 80th, 60th, 40th and 20th percentile of `Sum` according to the table below. You may refer to Listing 5.6 in the book.

|Grades|                         Condition                          |  
|------| ----------------------------------------------------------- |   
|  A+ | `Sum` `>=` the 80th percentile                              | 
|  A  | `Sum` `<` the 80th percentile, but `>=` the 60th percentile | 
|  B  | `Sum` `<` the 60th percentile, but `>=` the 40th percentile |
|  C  | `Sum` `<` the 40th percentile, but `>=` the 20th percentile |
|  D  | `Sum` `<` the 20th percentile                               |

#### Question 2.3
Write a function named `Grade`, whose input is the name of one student and output is the grade of him or her.

#### Question 2.4
Draw a pie chart of the grades: `A+`, `A`, `B`, `C` and `D` from `table` with label for each part of the pie chart. You may refer to Listing 6.5 in the book.

#### Question 2.5
Divide the students into five groups by the grades: `A+`, `A`, `B`, `C` and `D`. Describe the mean and standard error of test scores for each group. 

### Question 3
Based on the same dataset `grades.txt`, answer the following questions. 

#### Question 3.1
Regress `Math` on `Chinese` and `English`. Summarize the result and draw a diagnostic plot like Figure 8.6 in the book. See what conclusion you can draw from this plot. 

#### Question 3.2
Draw a histogram of the studentized residuals and superimposes a normal curve, kernel density curve and rug plot. You may refer to Listing 8.6 in the book, but not use that `residplot` function unless you know how it works.

### Notice
1. You need to send your solution in __PDF__ format to my email (xiaojunsunshine@126.com) before __Tuesday, 15th July 24:00__.
2. You are required to include both the **source codes** and results in the your solution. 
3. The questions are a bit too many. :sweat_smile: Just go ahead and give it a try. If you feel it's hard to finish all the questions, you can just finish some of them and send to me. 
4. I will write a solution for this assignment and explain it in detail in the next meeting of R Club. 
5. I hope you have fun while learning R. :blush:  :kissing_heart: 

<p>&nbsp;</p>
<p><a href="http://xiaojunsun.github.io/wise-r-club/">Return to the homepage.</a></p>
-----
<p></a>WISE R Club project is proudly maintained by <a href="https://github.com/XiaojunSun">XiaojunSun</a>.</p>