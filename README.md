# Education-Inequality-and-Socioeconomic-Factors
## Project Description
This project addresses inequality of educational opportunity in U.S. high schools. I will focus on average student performance on the ACT or SAT exams that students take as part of the college application process. I expect a range of school performance on these exams, but I want to know if school performance is predicted by socioeconomic factors.

## Data Description
This project utilizes two data sets EdGap_data.xlsx and ccd_sch_029_1617_w_1a_11212017.csv. The primary data set is the EdGap data set from [EdGap.org.](https://www.edgap.org/#5/37.892/-95.977) This data set from 2016 includes information about average ACT or SAT scores for schools and several socioeconomic characteristics of the school district. The secondary data set is basic information about each school from the [National Center for Education Statistics.](https://nces.ed.gov/ccd/pubschuniv.asp) This data set consists of basic identifying information about schools and can be assumed to be of reasonably high quality. 

## Data Preparation
The file titled 'Eloho's_Education_Inequality_Data_Preparation.ipynb', contains detailed steps I took to prepare data from the two original datasets to create the final model. I joined both datasets retaining only the most important data columns. Next, I inspected the dataset to identify and get rid of outliers that might affect the model. I did this by identifying data that fell out of the percentage boundary. I then carried out a train test split which would be used to compare models predicting the average ACT scores. Next, I used the iterativeimputer function to impute missing data in the train dataframe. Lastly, I exported both datasets as CSV's. Those files can be found in this repository under the names "training_df.csv" and "testing_df.csv".

## Data Analysis
For this analysis, I aimed to address the following questions: How do average ACT scores vary by state? How well can we predict students' ACT scores based on socioeconomic factors? After accounting for mean income, do other socioeconomic factors still significantly affect ACT scores? What factor contributes the most to ACT scores?
Using descriptive statistics, I explored the relationship between ACT scores and median income across different states. I also developed a multivariate regression model to predict ACT scores, incorporating variables such as the unemployment rate, the percentage of parents who attended college, marital status of parents, the ability to provide meals at lunch, and median income.
To assess the impact of the model type on prediction accuracy, I constructed an additional model using a standard regression tree. To determine which feature most significantly affected model accuracy, I sequentially removed different features and observed the changes in prediction performance.
Finally, I analyzed non-numerical data by creating a bar chart to visualize ACT scores by school type, aiming to gain further insights from this perspective. This analysis can be found in this repro with the title ' Education inequality Analysis.ipynb'


## Author
This project was created and carried out by [Eloho Okoloko](https://www.linkedin.com/in/elohookoloko/). 

## License
[MIT]([https://github.com/Eliokay/Education-Inequality/blob/main/LICENSE]) © Eloho Okoloko


