# school-district-analysis

## Overview
Analysis of a district's standardized test scores using Jupyter Notebook and Anaconda. The original analysis considered all students grade levels 9th-12th within the school district. However, the school board noticed some discrepancies in the 9th grade scores for Thomas High School, so a second analysis was done to determine the same data after removing the test scores for 9th graders in Thomas High School.

### The analysis covered the following:
 - An overall look at the district's students, average test scores, passing percentages, and budget.
 - A more in-depth look at each school individually by average test scores, passing percentages, and budget per student.
 - Student performance by grade level
 - School performance by spending
 - School performance by school size
 - School performance by type of school (District or Charter)


## Results

Here we will see a comparison of the data with and without the Thomas High School 9th graders' scores.

### Overall District Summary

- Original Results:
 
 ![image](https://user-images.githubusercontent.com/100869713/165191434-c6cedaff-3d25-4165-bf40-5ff9ae059a3b.png)

- Updated Results

![image](https://user-images.githubusercontent.com/100869713/165191464-bceed6c8-0291-420c-bd4f-6d6bc8e01737.png)


As demonstrated above, the overall test results for the district are lower without the potentially misrepresented scores from the Thomas High School 9th grade. The average math score dropped by .1, the average reading score remained the same, the percentage passing math dropped by .2%, passing reading by .1%, and overall passing by .3%

### Per School Summary (Thomas High School)

 - Original Results:
 
 ![image](https://user-images.githubusercontent.com/100869713/165192699-ab5fdbec-4535-4c77-8768-1d360c4ef068.png)


 - Updated Results (Removal of Scores Only):

![image](https://user-images.githubusercontent.com/100869713/165192633-0437bf39-c018-4275-b998-04e52ee6bb53.png)

 
 - Updated Results (Removal of Students):

 ![image](https://user-images.githubusercontent.com/100869713/165192737-be2ba537-f7ae-42ee-af95-386871033777.png)
 


 As demonstrated above, the impact of removing the 9th graders' scores is significant, a ~20-25% loss in all passing percentage categories. However, once we stop counting the 9th graders' among Thomas High School's population, their passing percentages shoot back up to the 90% range.
 
 ### Thomas High School relative to other schools
 
 - Original Top Five Schools
 
 ![image](https://user-images.githubusercontent.com/100869713/165187586-ba88a2c9-4fb6-458c-b74c-80ea05cac431.png)

 - Updated Top Five Schools

 ![image](https://user-images.githubusercontent.com/100869713/165187658-a2a8a71a-e213-42c2-afa5-d18e3a949f75.png)

As shown here, the removal of the 9th grade scores does not knock Thomas High off of the second slot, despite the reduction in averages and % passing.

### Thomas High School scores:

 - By Grade Level:

As the only change was the *removal* of all 9th grade scores from this school, the only demonstrable change is replacing the original 9th grade averages, 83.6 for Math and 83.7 for Reading, with a value of NaN, or "Not a number".

 - By School Spending:
 
  - Original:
 
 ![image](https://user-images.githubusercontent.com/100869713/165188418-6203284c-333e-43da-a258-e47df876343f.png)

  - Updated:
  
  ![image](https://user-images.githubusercontent.com/100869713/165188439-5640ce42-4c04-4f03-8bb9-6ce17b09b7bc.png)

There is no demonstrable difference in averages or passing percentages by school spending, after removing the Thomas High 9th graders. Thomas High is in the "$631-645" spending bin, which did not change at all after rounding.

 - By School Size:
 
   - Original:
   
  ![image](https://user-images.githubusercontent.com/100869713/165188682-ea7eb9fe-7e7a-4473-8942-4def41fb59c4.png)

   - Updated:
   
   ![image](https://user-images.githubusercontent.com/100869713/165188721-e8b800aa-8e19-40a8-bb58-3e55cfe37160.png)

 Thomas High School is a "Medium"-sized school. Just as above with spending, the scores and passing percentages did not meaningfully change.
 
  - By School Type:
  
    - Original:

    ![image](https://user-images.githubusercontent.com/100869713/165189013-b5c9d8f2-3b89-4977-973b-ded211687b42.png)

     - Updated

     ![image](https://user-images.githubusercontent.com/100869713/165189046-8c1b7341-78db-4ed4-a5eb-9327d88b9cb0.png)
     
     Thomas High School is a Charter School, and as demonstrated here, the removal of the 9th graders did not meaningfully change their averages or percentages either.
     
## Summary

There were several minor but impactful changes that came with the removal of the 9th grade scores from Thomas High, including:
 - A drop of >1% in overall passing percentages for the whole district.
 - A significant drop in passing percentages occured when the ninth grade students were still counted, but once they were removed (as they were not failing, just simply invalid), Thomas High still performed well.
 - Averages for Thomas High in Math and Reading rose by <1% each once the 9th grade students were removed.
 - Passing percentages for Thomas High in Math, Reading, and Overall, however, each fell by <1%.

 


