There are three main options to achieve the selection and indexing activities although there are multiple ways to select and index rows and columns from  Pandas Dataframes.<br/>
1.selecting data by row numbers(.iloc)<br/>
2.selecting data by label or by a conditional statement (.loc)<br/>
3.selecting in a hybrid approach(.ix)  <br/>

I’m going to write about the iloc indexer here because this indexing is suitable for 100-days-Of-ML challenge Day1 and Day2 problems. 
Selecting data by row numbers(.iloc).<br/>
According to its name “iloc”,it is used for interger-location based indexing/selection by position.<br/>- The syntax of iloc indexer is data.iloc [ row selection ,  column selection ]. <br/>-You can simply imagine that each row has a row number from 0 to the total rows(data.shape[0]) .<br/>- Based on these numbers, iloc[] allows selection .<br/>- The same applies for columns (from 0 to data.shape[1]). The different indexes of 0 and 1 in data.shape[] means that the first horizontal row can be denoted as “axis 1 ” and the first vertical column can be denoted as axis 0. 
  

  #Single selections using iloc and DataFrame

For  Rows:
   
    data.iloc[0] // first row of data frame 
    data.iloc[1] // second row of data frame 
    data.iloc[-1] // last row of data frame 

For Columns:

    data.iloc[:,0] //first column of data frame 
    data.iloc[:,1] //second column of data frame 
    data.iloc[:,-1] // last column of data frame 
  
#Multiple Columns and Rows Selection
   
    data.iloc[0:5] //first five rows of dataframe
    data.iloc[:, 0:2] //first two columns of data frame with all rows
    data.iloc[[0,3,6,24], [0,5,6]] //1st, 4th, 7th, 25th row + 1st 6th 7th columns.
    data.iloc[0:5, 5:8] //first 5 rows and 5th, 6th, 7th columns of data frame 


