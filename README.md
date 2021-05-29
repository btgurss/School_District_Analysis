# Py City School Analysis

## Overview/Purpose
The Py City School District is looking to analyze data from recent test scores.  In order to effectively use this data, the district wants it organized in a variety of ways.  The district wants to be able to determine if the size, type, or amount of spending has an impact on test scores.  They also want to compare the different grade levels of each school to see if certain grades perform better than others.

## Results
The City realized that data taken from the 9th grade students from Thomas High School was not reliable and that it needed to be removed from the data set (or at least counted differently).  When this happened, the data changed slightly.  Here are the changes:

- The district summary changed very little.  There were enough students in other schools to make it difficult for the overall results to change a large amount.  Each category saw the average scores and percents drop slightly after these results were removed.  This indicates the removed scores were generally higher than those in the original set.  The results are shown below.

District Summary Original
District Summary Replaced

- The school summary changed very little as well.  The Thomas High School average scores and percents were the only numbers that changed when the data was removed.  This is a good sign as that was the only data that was altered and if other school information did change it would show that the written code was incorrect.  Originally the averages for the Thomas High School dropped significantly as the averages for the school were calculated on the total students and we now had an entire grade of zeros.  Once I redid the code to account for the missing students the averages went back to close to where they were before.  They were not exact, but were close.

School Summary Original
School Summary Replaced

- As mentioned above, the performance of Thomas High School stayed about the same after the data was removed.  In both instances (with and without the 9th grade data) the school placed 2nd in overall passing percentage.  This percentage only dropped about .4 points and was not enough to move the school into a different placement.
The replacement of these scores also did almost nothing to any of the following categories
    - Scores by school spending
    - Scores by school size
    - Scores by school type
    - Math and reading scores by grade (There was a small change here as everything stayed the same except for the 9th grade Thomas High School data went from an actual score to NAN.)
This tells me that my written code is doing its job correctly, as none of these data sets should have been impacted by removing one small portion of data unless that data was far from the mean.

## Summary
Here is list of changes that occurred after the 9th grade Thomas High School math and reading scores were removed.

1. The math and reading scores by grade level were replaced by NaN.  This happened because there were no scores to find the averages of.
2. The math score averages for the school dropped by about .1.  This tells me that even though there was an error somewhere, the error may not have had a very big impact on the overall data.
3. The reading score averages increased by a small amount.  Interestingly, the percent of students who passed the reading section actually went down by a little.  This tells me that there may have been a few students who scored extremely well and helped bring up the average score and this was able to negate some of the students who did not pass.
4. The overall passing percentage went down about 0.3.  Once again, this tells us that the 9th grade students performed slightly better than the 10th - 12th graders.  This does not seem like a big enough difference for the school to remove the scores.  I would need more information to know the reasoning behind the removal.
