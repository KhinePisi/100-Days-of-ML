## Motivation
If we dont have any interest on the relationship between variables and fit it into a model, the results will be messy and meaningless, so here comes Correlation Coefficient. <br>
## Correlation Coefficient 
- It is used to determine how strong a relationship is between two variables.<br>
- returns value between (-1 and 1) <br>
- 1 indicates a strong positive relationship.( for every positive increase in one variable, there is a **positive increase** of a fixed proportion in the other)<br> Example: (the darker the night ,the more productive you become :v) 
- -1 indicates a strong negative relationship.( for every positive increase in one variable, there is a **negative decrease** of a fixed proportion in the other) Example:( the amount of gas in a tank decreases in (almost) perfect correlation with speed.)
- 0 indicates no relationship at all.(there isn’t a positive or negative increase. The two just aren’t related).
- Note that only the absolute value of the result can give us the coefficient strength . |-.75| = .75, which has a stronger relationship than .65.
- In linear regression,Pearson’s correlation is commonly used.<br>

There are several ways of finding coefficient formulas.I will describe the most basic one here . 
   ![Equation Image ](https://github.com/KhinePisi/100-Days-of-ML/blob/master/Correlation%20Coefficient.JPG)<br>
   Implementation of Equation <br>
   Step1. Choose two data columns you want to calculate ( two variables x and y)<br><br>
   Step2. Add another 3 columns ( xy , y*y ,x*x) <br>
            - Multiply x and y together to fill the xy column.<br>
            - Take the square of the numbers in the x column, and put the result in the x*x column.<br>
            - Take the square of the numbers in the y column, and put the result in the y*y column.<br>
   Step3. Add up all of the numbers in the columns and put the result at the bottom of the column.   <br>
   Step4. Use the correlation coefficient formula. <br>
            You can now analyze the results and decide whether you are going to find any statistcal equation with them or not . <br>
   
This is important in data analyzing and preprocessing steps especially for Linear Regression Models.<br>

   
   -------------------------------------------------------------------------------------------------------------------








