---
layout: default
title: Home
---

# Workshop: Stata Helpdesk

In this helpdesk you can ask questions about the use of Stata in your course or work through these questions.

<div class="instructions" markdown="1">
  
1. Open Stata
2. Download <a href="exploreschool.dta">here</a> the datafile
3. Open this file in stata

The data contains some information recorded by a school several years ago.

4. Use the command `br`
5. Comment on what is contained in the dataset.
6. Use the `table` command to find how many students were each of the year groups recorded.
 
</div>

<div class="explanation" markdown="1">

The `table` command can be used with the following syntax:

`table` Variable_Name

</div>

<div class="instructions" markdown="1">
  
  7. How many female and male students wre recorded in this dataset?
  8. Use the `summarize` or `sum` command to get summary statistics for **height**, **weight**, **TV hours**, and **IQ**
  9. To the beginning of your `sum` command add `by YearGroup, sort:`

`by YearGroup, sort:` List_of_Variables

</div>

<div class="instructions" markdown="1">
  
  ### Scatter diagrams

  10. Create a scatter diagram of TV hours against IQ for the year 10 group using:

      `twoway (scatter IQ TV if YearGroup == 10`

11. What happens to the scatter graph if you put the `IQ` and the `TV` the other way around?
12. Create a scatter diagram of TV hours against IQ for the year 11 group.
13. Find the **correlation coefficient** between the height and the weight variables.  Use the `pwcorr` command/
14. Is the sign of the correlation what you would expect?
15. Add `, sig` to the end of the correlation command to determine whether the correlation is **significant**
    
</div>

<div class="instructions" markdown="1">
  
  ### Histogram

  16. Create a **histogram** to the show the distribution of IQ scores.  Use the command `histogram IQ`
  17. Does there appear to be any errors in the dataset?
  18. Create a histogram to show the distribution of weekly tv hours.
  19. Does there appear to be any skew within the tv hours data?

</div>

<div class="instructions" markdown="1">

  ### T-test

20. Carry out a t-test to determine whether there is any significant difference between the heights of the two year groups.

</div>

<div class="explanation" markdown="1">

The t-test syntax is:

`ttest `Test_Variable, `by (` Group_Variable `)`
</div>
