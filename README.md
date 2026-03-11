# Student Productivity and Behaviours Project

This project is a comprehensive data analysis tool designed to streamline data exploration, analysis, and visualisation. The tool supports multiple data formats and provides an intuitive interface for both novice and expert data scientists.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

Live Dashboard link on PowerBI: https://app.powerbi.com/groups/me/reports/9b54216b-0cc0-4e16-94c1-ccf61d4863f7/ea084256ccc05733c726?experience=power-bi

## Dataset Content

I chose my own dataset called Student Productivity & Behavior which I found on Kaggle, please see the link below;

https://www.kaggle.com/datasets/algozee/student-productivity-and-behavior-dataset-20k

The Student Productivity & Behaviour Dataset (20K) contains 20,000 structured student records that capture information related to study habits, digital usage patterns, wellness indicators, productivity metrics, and academic results.

Features: daily study hours, smartphone and social media usage, sleep duration, stress levels, focus scores, productivity scores, attendance, and final grades. It enables comprehensive analysis of how different behavioural and lifestyle factors collectively influence students’ productivity and academic success, making it suitable for exploratory data analysis, predictive modelling, and educational research.
Derived Features: Wellness score, Screen time.
Personal reasons: I decided to use this dataset instead of one of the options provided to us because I personally relate to its subject matter. Having returned to education after a long period away, I am particularly interested in understanding how various factors and lifestyle choices can influence students. This dataset offers valuable insights into these effects, which aligns closely with my own experiences and interests

## Business Requirements and Map to Data visualisations

This Project has four business requirements.
BR1: Identify key factors that can cause high stress levels and analyse how these will affect a student’s final grade, focus and productivity scores.

Data visualisation: The correlation matrix was applied to calculate the Pearson correlation coefficient between the variables in the dataset. 

Stress vs Productivity = -0.197 – weak relationship.
Stress vs Final grade = -0.012 – no relationship.
Productivity vs Final grade = no correlation.
Barplots were chosen to present the data showing that the higher the productivity score the lower the stress level.

BR2: How do patterns of phone usage and social media consumption affect students’ focus and overall productivity scores?

Data visualisation: A scatterplot was used to illustrate that relationship between social media consumption and focus and productivity scores by using the new column created Screen time.

BR3: How do variations in sleep duration, exercise frequency and wellness practices influence a students’ stress levels?

Data visualisation: A scatterplot and heatmap was used to demonstrate the variations between sleep, exercise and stress levels using the new column created Wellness scores.

BR4: What is the relationship between students’ daily study hours and attendance with their final grades?

Data Visualisation: A scatterplot and heatmap were used to predict final grades. However, the predictions were inaccurate, as the analysis indicated that daily study hours and attendance had no measurable impact on students' final grades.

## Hypothesis and Validation

This project analysed three hypotheses regarding student behaviours. 
HYP1: Students with higher attendance rates are more likely to achieve a higher final grade. 
Revised HYP1: Students with higher attendance rates are more likely to have a higher productivity score.
Validation: Scatter plots (visual validation)
Results: The scatter plot generated for this analysis demonstrates a general upward trend. This indicates that students with higher attendance rates tend to achieve higher productivity scores. While the data points on the scatter plot are closely clustered, making it difficult to distinctly observe individual relationships, the overall direction of the plot still suggests a positive association between attendance and productivity. This pattern provides support for the revised first hypothesis, which proposes that students who attend more frequently are likely to be more productive.

HYP2: Increased social media content is to negatively influence a students’ focus and productivity levels.
Validation: Scatter plots (visual validation)
Results: The scatterplot indicates that increased social media consumption is somewhat correlated with reduced productivity scores. However, the relationship between social media usage and focus scores is inconclusive and cannot be clearly characterized as either positive or negative.

HYP3: Higher levels of Sleep and exercise will reduce the stress levels among students.
Validation: Heatmap
Results: Disapproved: The heatmap shows that the value 0.0026 is very close to 0, indicating that there is no correlation between these two variables.

HYP4: Null Hypothesis H0:  There is no difference in the final grades of students who study less than four hours per day than those who study more than four hours.
Alternate Hypotheis Hₐ : Students who study more than four hours per day will have a have a higher final grade.
Validation: T-test
Result: T-statistic: -1.0152027043599512
P-value: 0.31002149386245886
The p-value is 0.31 is greater than 0.05 (standard significance level), we fail to reject the null hypothesis. The data does not provide sufficient evidence.

## Project Plan

ETL Process – Load the dataset taken from Kaggle into VS code.

Transform the data by the cleaning process; missing values, duplicates and outliers.
Encoded categorical variables using one hot encoder.
Created two new features: Screen time; grouped social media hours, gaming hours, youtube hours and phone usage hours.
Wellness score: grouped sleep hours and exercise time.

Loading the cleaned data in to the appropriate files and folders so it can used for data analysis.

Data Analysis: conducted descriptive statistics such as mean, median, standard deviation. 
Visualisation of data: Using scatterplots, boxplots and barplots to identify key correlations between the different variables.
In depth Data Visualisation: Using scatter plots and heatmaps to examine relations and correlations that relate back to my busiess requirements and hypotheses.

Reports:
Consistently reported progress and maintained comprehensive documentation throughout the project's duration.

## Analysis techniques used

Structured approach: I structured the data analysis technique by following the module handbook and going through each criteria to add to my project, this included reviewing each section. By adhering to the handbook's guidance, I was able to incorporate all necessary elements and maintain consistency throughout the analysis process.
Data limitations: The data did not present any limitations; however, it could have been more of a challenge. There were no missing values or duplicates, which streamlined the data cleaning process. Additionally, there was only one categorical variable which I could not conduct in-depth analysis on categorical data.
Generative AI: I used AI to help with the code and ideas which helped me immensely throughout this project.

## Ethical considerations

 No ethical considerations in this project.

## Dashboard Design

Dashboard Design:
🏠 HomePage
💬 Social Media Usage
🪷 Wellbeing
💡 Insights

•Interactive Filters and slicers: Allow users to filter data by relevant attributes. Created navigation panel to help users to access the different pages. I added hover and icons to the navigation panel for user interactions. Added slicers to allow users to narrow down the data.
•Dynamic Charts and Graphs: Include various chart types such as cluster bar charts, pie charts 
•Predictive Insights: Provided detailed insights to users by using tooltips on every page.
•Storytelling: Create a narrative that guides users through the key findings and insights from the data.

## Unfixed Bugs

All bugs in this project have been resolved; there are no outstanding issues remaining.

I recognized gaps in my knowledge with certain topics such as feature engineering and machine learning. I addressed these by going back to the LMS and refreshing my knowledge. I watched youtube videos and visited websites such as GeeksforGeeks to help me gain a better understanding of these topics.
I used auto completion in VS code, chatgpt, co-pilot and gemini to help with the code.
I also used co-pilot to help me structure sentences in a formal way when writing Markdown and README documentation.

## Development Roadmap

Challenges faced with this project:

1.Organizing Data Files and Folders
 One challenge faced during the project was organizing both clean and raw data files and folders within VS Code. This issue was addressed by seeking assistance from Vasi, who reorganized the files in a more efficient way, making data management smoother.

2.Loading and Saving Data
Difficulties arose when trying to load raw data and save processed data. The raw data issue was resolved by experimenting with the dataset and utilizing auto-completion features in VS Code. However, saving the data required further support. ChatGPT provided guidance on using an absolute pathway and the project_root directory, which enabled successful saving of the dataset.

3.Feature Engineering Oversight
A feature engineering step was initially missed and had to be added later during project review. To resolve this, additional feature engineering was incorporated into the ETL notebook. Guidance on selecting the appropriate one-hot encoder for this project was obtained by consulting the GeeksforGeeks website.

4.Revision of Hypotheses
While working through the core concepts, a hypothesis was revised and another was added. These updates were reflected in the ETL notebook to ensure that the analysis remained thorough and accurate.

## Learning Journey and Reflections

I will learn new features and designs on PowerBI to make the dashboard more dynamic and extensive. 
I will learn best practices for next project.
In reflection, I realised that my initial preparation and time management could have been improved. While I did make efforts to plan my approach, I found that I spent too much time before actually executing the tasks. To organize my thoughts and lay out a clear path, I utilised both my notebook and a Word document to draft a plan for preparing my project and outlining the features for the dashboard. Despite this planning, I feel that I could have benefited from acting more promptly and efficiently. This reflection highlights the importance of not only planning ahead but also ensuring that the plan is implemented in a timely manner.

## Main Data Analysis Libraries

Numpy and Pandas – used for data processing
Matplotlib and Seaborn – used for data visualisation.
sklearn.cluster import KMeans and sklearn.preprocessing import StandardScaler – for Machine Learning
from sklearn.preprocessing import OneHotEncoder – for feature engineering
Statistical tests – used for statistical analysis
PowerBI – used for Dashboard.

## Credits/Content

The dataset was taken from Kaggle - Student Productivity & Behavior Dataset (20K)
The explanation and code was taken for feature engineering was taken from One Hot Encoding in Machine Learning - GeeksforGeeks
The invisible character used in my Dashboard was taken from Invisible Character 
https://www.editpad.org/tool/invisible-character

Instructions on how to create a navigation menu was taken from https://youtu.be/-GCV4LvPMW0?si=4Nw9dr73c6wEZY4S

Understanding and creating the code for K-means clustering were inspired by:
https://www.geeksforgeeks.org/machine-learning/k-means-clustering-introduction/#google_vignette

[2.3. Clustering — scikit-learn 1.8.0 documentation](https://scikit-learn.org/stable/modules/clustering.html)

[Python Machine Learning - K-means](https://www.w3schools.com/python/python_ml_k-means.asp)

[Code Institute - Advanced Data Analysis Techniques](https://lms.codeinstitute.net/learner_module/show/118491?lesson_id=506369&section_id=1920594)

To reinforce my understanding of key concepts, I utilized the Learning Management System (LMS) to revisit certain topics. This process allowed me to refresh my memory and ensure a stronger grasp of relevant material needed for the project.

### Media

No external media used.

## Acknowledgements

I would like to thank my course coordinators, Vasi and Mark for providing help in preparing the project and support through this project.
