# Education-Inequality-and-Socioeconomic-Factors
## Project Description
This project addresses inequality of educational opportunity in U.S. high schools. I will focus on average student performance on the ACT or SAT exams that students take as part of the college application process. I expect a range of school performance on these exams, but I want to know if school performance is predicted by socioeconomic factors.

## Data Description
This project utilizes two data sets EdGap_data.xlsx and ccd_sch_029_1617_w_1a_11212017.csv. The primary data set is the EdGap data set from [EdGap.org.](https://www.edgap.org/#5/37.892/-95.977) This data set from 2016 includes information about average ACT or SAT scores for schools and several socioeconomic characteristics of the school district. The secondary data set is basic information about each school from the [National Center for Education Statistics.](https://nces.ed.gov/ccd/pubschuniv.asp) This data set consists of basic identifying information about schools and can be assumed to be of reasonably high quality. 

## Data Preparation
The file titled 'Eloho's_Education_Inequality_Data_Preparation.ipynb', contains detailed steps I took to prepare data from the two original datasets to create the final model. I joined both datasets retaining only the most important data columns. Next, I inspected the dataset to identify and get rid of outliers that might affect the model. I did this by identifying data that fell out of the percentage boundary. I then carried out a train test split which would be used to compare models predicting the average ACT scores. Next, I used the iterativeimputer function to impute missing data in the train dataframe. Lastly, I exported both datasets as CSV's. Those files can be found in this repository under the names "X_train.csv" and "X_test.csv".


