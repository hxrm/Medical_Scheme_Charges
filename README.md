## Analysis Plan 
The objective of this analysis is to create a linear regression model to accurately predictive insurance charges for a medical scheme member. The predictions will be based the observed selection of lifestyle factors for a client. Namly factors such as age, sex, BMI, number of children, smoking habits and geographical region. 
The analysis will include steps to understanding both the individual and combined implication of lifestyle factor on insurance charges for a medical scheme member. Will uncover the lifestyle factors that are both significant and irrelevant to the increase in insurance chargers and primarily build a model to generate insurance chargers. 
## Explanatory Data Analysis (EDA): 
Data exploration is a crucial step that needs to be taken before attempting to build a model. EDA helps an analysist to understand the given data. The EDA process identifies issues that may affect machine learning, ensures that data will be of suitable quality and identifies key patterns and trends that may need to be taken into consideration when building a predictive model (Ray, 2024). Various functions from the Pandas, Seaborn and Matplotlib libraries will be used to assist the EDA process. The EDA will include the following steps.

**Data Collection** : The first step to analysing the data is to retrieve it from the given csv file. The Pandas.read_csv() method will be used to read the data from the file and store is within a Pandas data frame object. The Pandas data frames can hold huge amount of data in excel like format, making it ideal to store insurance dataset and perform data manipulation (NumFOCUS Inc, 2024). 

**Data Cleaning**: To help ensure data quality missing vales, duplicates and inconsistencies in data types must be handled.
- Missing Values: panda.isnull().sum() will be used to search the dataset and return the sum of missing values for each column. Identified values will either be dropped or replaced with relevant columns average.
- Duplicated data: panda.duplicated() will be used to identify and create a list of all duplicates within the dataset. The list of duplicates will then be removed from the dataset to avoid introducing bias. 
- Data type consistency: panda.info() will be used to identify data types in the given dataset. This is important to ensure all data is numerical and as input for a linear algorithm. Data types that are not quantitative will be encoded or transformed to numeric form.   
**Data Transformation**: To use machine learning algorithms, all data must be in numerical form, either float or int data types. The categorical features sex, smoker and region must therefore be transformed. 
- Encode data: Features in the dataset that are the object data type will be encoded to transform to numeric form. LabelEncoder from the Scikit-learn preprocessing module will convert the values within sex, smoker and region features. The features will contain numbers to label each different category (Novogroder, 2024).
    
## Univariate Analysis: 
This stage of analysis focuses on analysing a single feature of the dataset at a time. Depending on whether a feature is categorical or numerical the analysis will differ (Ray, 2024). For features that are continuous values, assessment will include statistical summary to understand the distribution, central tendency and the variability for each feature within the dataset (Ray, 2024). Features that are categorical the frequency and count of the feature will be assessed using visualisation such as bar chart or count plots (Ray, 2024). 

## Bivariate Analysis: 
This stage of analysis focuses on two variables, to uncover the association and distribution between them (Ray, 2024). To understand the relationship between two variables visualisation tools such as seaborn and matplotlib will be used to create correlation heatmaps, pair plots, distribution plots and scatterplots.

## Multivariate Analysis:
This is analysis extends the bivariate analysis but is carried out on more than two features. The analysis stage is aimed at understanding the relationship between multiple variables. Tools from seaborn and matplotlib will be used to visualise the relations between variables. Plots such as distribution plots and scatterplots will carry out this stage (Deepanshi, 2023; KIm, 2023). 

## Pre Processing: 
Preprocessing are the final tasks that must be carried out to ensure that the data meets all requirements to be useful machine learning purposes (Novogroder, 2024). Tasks include scaling, encoding and splitting data to ensure that the model performs well (Novogroder, 2024). This stage will include various modules from the Scikit-learn library to prepare the data for processing.
**Data scaling**:Each feature in the dataset may have a different scale, this leads the model  to perceive features with larger values to have greater significance and produce inaccurate predictions. Scaling the dataset ensure that features have fair contribution. The Scikit MinMaxScaler() and StandardScaler() methods will be considered to scale the features within the dataset (GeeksforGeeks, 2025a).  
**Feature Selection**: Feature selection will be performed through either backward elimination or sklearn.selectKBest(). This is important as to only include features that offer meaning contribution to the prediction. By only including significant  features the performance and accuracy of the model will be enhanced(Imarticus, 2024) .
**Splitting data**: Data will be split before input into model. The data will be split into an 80:20 ratio, 80 percent of the data being used as training data and the remaining 20 percent for test data. This is an important step so that after training the model can be tested on unseen data to assess its performance (Gillis, 2024). 
## Build and Evaluate Model
**Model training**: The models used for this analysis will be the Scikit-learn Linear Regression model and Lasso Regression model. Linear Regression model has been selected as the native model to apply a linear regression algorithm. Lasso selected for its built-in feature selection capabilities (Orange Data Mining Library, 2015). 
**Evaluation**: To evaluate the performance of the models, the Scikit-learn library will be used. The library contains a metrics methods that provide the coefficient of determination (R^2) , mean absolute error and mean squared error for the results or prediction of a trained model (Deepanshi, 2023; Kim, 2023)  These metrics can be used to assess the performance and accuracy of a model.
**Visualisation of results**: Seaborn and Matplotlib will be used to display the result (Deepanshi, 2023; KIm, 2023). Plots such as  
- True vs Predicted Values, to compare predictions to actual datapoint and assess linearity   
- Residuals vs Predicted Values, to assess the Homoscedasticity of model of model results. 
- Normal Q-Q Residual Plot, to assess if residuals are normally distributed  
## Account Creation
![image](https://github.com/user-attachments/assets/ad999f14-c608-4595-9a18-e6b5d9e34319)

### Navigating to Registration:
   - Find and click on the "Register" link on the login page. 

### Complete Registration Form:
-	Fill in the required information and click on register to create your account.
-	Enter your name, surname, email address, and choose a secure password.
![image](https://github.com/user-attachments/assets/92ced83d-8af2-4b1f-861c-31fc27da5d8f)

### Submission:
   - Click the "Register" button to create your account.

![image](https://github.com/user-attachments/assets/a849837d-f72d-40a0-a13f-9406c0d02269)

## Logging In
![image](https://github.com/user-attachments/assets/7ecbfde8-0ef2-4a9f-9942-9ca82eb8d03a)

 
Open the website:
-	Open your preferred web browser.
-	Enter the website's URL.
At the Login Page and enter your credentials:
-	Input your registered email address and password in the respective fields.
-	Click Login."
-	![image](https://github.com/user-attachments/assets/8fa747e1-ddbf-4104-9bee-37cde1fe21d6)

 
## Home Dashboard Overview
### Home Dashboard
Upon logging in, you will see the home dashboard page which serves as the central hub with links to key sections of the website and module functions. 
![image](https://github.com/user-attachments/assets/5a5a7478-3ce1-490f-b61b-f19c80221646)
 
## Navigation
Use the navigation menu to access different sections of the website.
Navigation:
   - Easily navigate to “Create New Module”, ”View Modules”, “Record Study Modules” “View Study Progress” or “View Study Progress Graph”.

## Module Creation
### Accessing Module Creation
Navigate to the "Create Module" section”
-	Click on "Create New Module." Via the home page or navigation menu.
![image](https://github.com/user-attachments/assets/dd1df736-307c-4261-8fb0-d5a9f5618a36)

 
### Semester Details
When creating a module for the first time, you'll be prompted to provide your semester details:
-	Fill in module details such as start date, end date, and any additional information.
	![image](https://github.com/user-attachments/assets/294b70a3-bed1-4561-bb41-ddc1811cb864)
 
### Creating a New Module
Fill in module details in the form page:
-	Module Code, enter a unique code for the module (e.g., PROG6212).
-	Module Name, supply a descriptive name for the module (e.g., Programming 2B).
-	Number of Credits, specify the credit value for the module (e.g., 15).
-	Class Hours per Week, indicate the number of hours of in-class instruction per week (e.g., 5).
  ![image](https://github.com/user-attachments/assets/33de4be2-a4fa-4c64-8ef8-3d1588dec687)

 
### Saving and Submitting
To save module click “Create Module” and then “Next” to return to homepage.
Click “Create Module”:
-	Continue creating module by entering the new module data within the form or click “Next” if done.
  ![image](https://github.com/user-attachments/assets/440cf95e-c617-452e-af89-90ecbea59c91)

Confirmation Message: A confirmation message will appear, acknowledging the successful creation of the module.
![image](https://github.com/user-attachments/assets/88d7d2ec-d50e-45d3-a060-b22542e4dd97)

 

## Module Viewing
### Accessing Modules
Navigate to the "View Modules" section to see a list of all modules for the semester.
 ![image](https://github.com/user-attachments/assets/57844fd9-cd32-4878-bd3c-a7cd57a4def7)


## Record of Studied Hours

To record your studied hours for a specific module, follow these steps:

### Record Studied Hours for a Module: 
Navigate to the " Record Study Hours " section and select the desired module from the dropdown list.  
![image](https://github.com/user-attachments/assets/43fdb103-e0de-4ed0-9222-247c61d2db06)

 ![image](https://github.com/user-attachments/assets/98b40203-503f-4d29-890a-eb7bf31d3620)



### Select Date:
Input or click on the calendar icon and a calendar interface will appear. Select the date you want to record your study hours for.
  ![image](https://github.com/user-attachments/assets/c47a6469-3052-4d3d-a2d1-7602466e5b6b)

![image](https://github.com/user-attachments/assets/9dfa4a7e-2a21-4d47-9277-5dbd73f99a4b)

### Input Study Hours:
Once the date is selected, input the number of hours you dedicated to studying for that session.
 
![image](https://github.com/user-attachments/assets/91b26a80-69cd-40f7-afaa-3769e0c02d07)

 
### Save:
Click the "Save" button to confirm and save your recorded study hours.
 ![image](https://github.com/user-attachments/assets/87733b2e-c938-4112-bbca-aa2175074a2f)

Confirmation Message: A confirmation message will appear, acknowledging the successful recording of your study hours.
![image](https://github.com/user-attachments/assets/0daf53b5-34dc-4a65-8e28-a0ddbf248592)

 
This process allows you to precisely record your study efforts for each module on specific dates. The dropdown list, calendar interface, and confirmation message enhance user experience and provide a systematic way to keep track of your study sessions. 


### Weekly Study Progress
Navigate to the " View Stud Progress " section and select the desired module and week to display.
5.4.1 Selecting Module and Week
 Module Selection:
-	Use the dropdown list to select the module you want to review.
  ![image](https://github.com/user-attachments/assets/038e8a17-b077-41d9-92b9-8ab93c5b5072)

 
Week Selection:
-	Choose the specific week you want to analyze from the dropdown box.
-	 ![image](https://github.com/user-attachments/assets/563fa5ef-5d82-4b26-a61a-2d0107a7e22b)

### Displayed Information
After selecting the module and week, the following information will be displayed:
-	Module Code, the code associated with the selected module.
-	Hours Studied, the total number of hours you have studied for the selected module during the chosen week.
-	Remaining Hours, the remaining hours recommended for study based on your ideal study hours and the current week's progress.
-	![image](https://github.com/user-attachments/assets/430e53f6-50f1-4ae7-b06f-25672196376e)
-	![image](https://github.com/user-attachments/assets/296d1a3e-e1f8-47ae-b12f-76480b70be10)

 
 

This detailed breakdown provides a focused view of your study efforts for a specific module during a particular week, helping you manage your time effectively and stay on top of your academic commitments.


## Module Study Progress Graph 
Navigate to the "View Study Progress Graph" section and select the desired module to display.
![image](https://github.com/user-attachments/assets/639f7e9e-0e53-44a2-8d51-8726ac89a9fc)

 

### Selecting Module
Module Selection:
-	Use the dropdown list to select the module you want to review.
-	 ![image](https://github.com/user-attachments/assets/9063e732-433b-4143-8c17-42b1b12d2c39)


### Displayed Graph
After selecting the module, the system will display a bar graph representing the study progress for the chosen module.
![image](https://github.com/user-attachments/assets/14206d16-7516-45e7-8ca8-77877ac366ad)

 ![image](https://github.com/user-attachments/assets/0171d0d7-a12b-46ce-a06d-4f4b489ae46b)


Graph Information:
•	Y-Axis (Hours): Represents the total number of hours studied.
•	X-Axis (Weeks): Indicates the weeks under consideration.
Graph Elements:
•	Actual Hours of Study: The bars will show the actual hours of study completed for each week.
•	Ideal Study Hours: A reference line on the graph will indicate the ideal study hours for each week.
 
![image](https://github.com/user-attachments/assets/ac065bf5-c757-409d-9975-2076ae67d9be)

### Information Overlay
Additionally, the page will display a key for the graph and hovering over each bar on the graph will display detailed information:
•	Week: The specific week in consideration.
•	Actual Hours of Study: The exact number of hours studied during that week.
•	Ideal Study Hours: The recommended ideal study hours for that week.
![image](https://github.com/user-attachments/assets/31a45397-c5fe-4538-9e89-e2b0e84d1005)


 
This graphical representation provides a visual insight into your study progress, allowing you to compare your actual study hours with the recommended ideal study hours. It helps in identifying trends, evaluating consistency, and making informed adjustments to your study routine.

# Student Study Hub

## Overview

Student Study Hub is a ASP.NET Web Application Console App developed on the .NET framework 4.8.
Student Study Hub is a web-based application designed to enhance the academic experience of students by providing tools to manage and optimize their study routines for the semester. This application allows students to seamlessly input and manage details of their modules, track study hours, monitor their progress throughout the semester and view their progress.
The Study Tracker Application serves as a valuable tool for enhancing the learning experience throughout the semester. 
THE WEBSITE NO LONGER AVALIBLE ON THE AZURE, AS SCHOOL PROVIDED HOSTING SERVIES HAVE BEEN DEACTIVATED 


## Usage
The Student Study Hub application is designed to help you effectively manage your semester by tracking module information and study hours. Follow these step-by-step instructions to make the most out of the application:
### User Account 
Register an Account: 
Before utilizing the web application's features, create an account.Upon launching the website, land on the login page with navigation to register an account if not already registered.
-	To login a user will be required to input their email address along with an formatted password.
-	To register a user will be required to input their name, surname, email address and password. If the email address has not been registered an account will be created.

### Creating Modules
1.	Launching the Website: 

Users can add modules for the semester by navigating to the "Create Module" section either located on the navigation bar or on the home page to add modules for your current semester.

2.	Enter Semester Data:
Set the start date for the first week of the semester, choose the start date for the first week of the semester by clicking on the calendar icon and selecting the date in the calendar view.

Enter the total number of weeks in the semester.
3.	Enter Module Information:
On the “Create Module” page, provide the following details for each module:
- Module Code:** Enter a unique code for the module (e.g., PROG6212).
- Module Name:** Supply a descriptive name for the module (e.g., Programming 2B).
 - Number of Credits:** Specify the credit value for the module (e.g., 15).
  - Class Hours per Week:** Indicate the number of hours of in-class instruction per week (e.g., 5).

4. Saving Module Information:
   - Once you've filled in the module details, click the "Save" button to store the module information.

### Tracking Study Hours
Recording Study Hours:
To record the number of hours spent studying a specific module on a particular date, navigate to the "Record Study Hours" page from the navigation bar or home page. Follow these steps:
-	Select the module you wish to update from the dropdown list on page.
-	Select the “Study Date” from the calendar from the view by clicking on the calender icon and selecting the date. 
-	Enter the “Studied Hours” by input the hours devoted to studying for the module in the textbox.
-	Click "Save" to record your study hours.

### Monitoring Progress
Viewing Module Information:
The application automatically calculates and displays the number of self-study hours required for each module per week based on the provided data. To access this information, select the "View Modules" from the navigation bar or homepage. This feature assists you in planning your study schedule effectively.

Monitoring Remaining Self-Study Hours:
The software continuously updates and displays the remaining self-study hours for each module for the current week. You can access this information by selecting "Study Progress " from the navigation bar or homepage. The calculation considers the hours recorded on specific dates to provide an accurate overview of your progress. On the Study Progress page,
-	Select the module you wish to view from the dropdown list on page.
-	Select the study week you wish to view from the dropdown list on page.
-	Module hours for the chosen week will be display, click "Home" to return to home page.


### Application Behavior

Data Storage on Azure:
Student Study Hub leverages Azure SQL Database for robust data storage to maintain data persistence. All user-related information, including usernames and securely hashed passwords, is stored in the designated Azure SQL Database. This cloud-based solution ensures data reliability, scalability, and accessibility.

.

User Registration and Password Management on Azure:
Users can seamlessly register within the application using a unique username and password. The application employs a secure approach by storing only the hash of the user's password in the Azure SQL Database. This cryptographic method enhances security by preventing the storage of sensitive information in plain text.

Exiting the Application:
Users enjoy the flexibility to perform various actions within the application hosted on Azure. The application ensures a smooth exit process, allowing users to securely log out, terminate their session, or exit the application altogether. This enhances the overall user experience and ensures the security of user interactions on the Azure platform.


## References
Ajaykumar, 2024. Data Science: Guide to Encoding Nominal Categorical Features. | by Ajaykumar Dev | Medium. [online] Available at: <https://medium.com/@nikaljeajay36/data-science-guide-to-encoding-nominal-categorical-features-bf3e622b1133> [Accessed 23 April 2025].
Akinkugbe, A., 2024. When to Use Linear Regression. Introduction | by Ayo Akinkugbe | Medium. [online] Available at: <https://medium.com/@ayoakinkugbe/when-to-use-linear-regression-6b7057ebd01f> [Accessed 23 April 2025].
Anomalo, 2024. Best Practices for Data Quality in Machine Learning. [online] Available at: <https://www.anomalo.com/blog/data-quality-in-machine-learning-best-practices-and-techniques/> [Accessed 24 April 2025].
Bechtel, M., 2025. Measuring the Strength of Linear Associations with a Correlation Coefficient | Statistics and Probability | Study.com. [online] Available at: <https://study.com/skill/learn/measuring-the-strength-of-linear-associations-with-a-correlation-coefficient-explanation.html> [Accessed 25 April 2025].
Bevans, R., 2020. Simple Linear Regression | An Easy Introduction & Examples. [online] Available at: <https://www.scribbr.com/statistics/simple-linear-regression/> [Accessed 25 April 2025].
Bhandari, A., 2025. Multicollinearity Explained: Causes, Effects & VIF Detection. [online] Available at: <https://www.analyticsvidhya.com/blog/2020/03/what-is-multicollinearity/> [Accessed 25 April 2025].
DATAtab Team, 2025. Linear Regression: A Complete Guide to Modeling Relationships Between Variables. [online] Available at: <https://datatab.net/tutorial/linear-regression> [Accessed 25 April 2025].
Deepanshi, 2023. Linear Regression | Introduction to Linear Regression for Data Science. [online] Available at: <https://www.analyticsvidhya.com/blog/2021/05/all-you-need-to-know-about-your-first-machine-learning-model-linear-regression/> [Accessed 25 April 2025].
GeeksforGeeks, 2024. Assumptions of Linear Regression | GeeksforGeeks. [online] Available at: <https://www.geeksforgeeks.org/assumptions-of-linear-regression/> [Accessed 25 April 2025].
GeeksforGeeks, 2025a. Feature Engineering: Scaling, Normalization, and Standardization | GeeksforGeeks. [online] Available at: <https://www.geeksforgeeks.org/ml-feature-scaling-part-2/> [Accessed 25 April 2025].
GeeksforGeeks, 2025b. Multiple Linear Regression with Backward Elimination | GeeksforGeeks. [online] Available at: <https://www.geeksforgeeks.org/ml-multiple-linear-regression-backward-elimination-technique/> [Accessed 25 April 2025].
Gillis, A., 2024. What is data splitting and why is it important? [online] Available at: <https://www.techtarget.com/searchenterpriseai/definition/data-splitting> [Accessed 25 April 2025].
Gorelick, M.H., 2006. Bias arising from missing data in predictive models. Journal of Clinical Epidemiology, [online] 59(10), pp.1115–1123. https://doi.org/10.1016/j.jclinepi.2004.11.029.
Imarticus, 2024. A Guide to Feature Selection for Linear Regression Models. [online] Available at: <https://imarticus.org/blog/linear-regression-models/> [Accessed 25 April 2025].
Kavya D, 2023. Optimizing Performance: SelectKBest for Efficient Feature Selection in Machine Learning | by Kavya D | Medium. [online] Available at: <https://medium.com/@Kavya2099/optimizing-performance-selectkbest-for-efficient-feature-selection-in-machine-learning-3b635905ed48> [Accessed 25 April 2025].
KIm, D., 2023. How to plot Predicted vs Actual Graphs and Residual Plots | by Dooinn KIm | Medium. [online] Available at: <https://dooinnkim.medium.com/how-to-plot-predicted-vs-actual-graphs-and-residual-plots-dc4e5b3f304a> [Accessed 25 April 2025].
Minitab, 2024. What are categorical, discrete, and continuous variables? - Minitab. [online] Available at: <https://support.minitab.com/en-us/minitab/help-and-how-to/statistical-modeling/regression/supporting-topics/basics/what-are-categorical-discrete-and-continuous-variables/> [Accessed 23 April 2025].
Novogroder, I., 2024. Data Preprocessing in Machine Learning: Steps & Best Practices. [online] Available at: <https://lakefs.io/blog/data-preprocessing-in-machine-learning/> [Accessed 25 April 2025].
NumFOCUS Inc, 2024. pandas.DataFrame.corr — pandas 2.2.3 documentation. [online] Available at: <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.corr.html> [Accessed 25 April 2025].
Orange Data Mining Library, 2015. Regression (regression) — Orange Data Mining Library 3 documentation. [online] Available at: <https://orange3.readthedocs.io/projects/orange-data-mining-library/en/master/reference/regression.html> [Accessed 25 April 2025].
Ray, S., 2024. A Guide to Data Exploration, Steps Data Analysis - Analytics Vidhya. [online] Available at: <https://www.analyticsvidhya.com/blog/2016/01/guide-data-exploration/#h-what-is-data-exploration> [Accessed 25 April 2025].
Saxena, S., 2024. What are Categorical Data Encoding Methods | Binary Encoding. [online] Available at: <https://www.analyticsvidhya.com/blog/2020/08/types-of-categorical-data-encoding/> [Accessed 23 April 2025].
Singh, P., 2023. How do outliers impact linear regression evaluation? [online] Available at: <https://www.linkedin.com/advice/3/how-do-outliers-impact-linear-regression-dz0ff> [Accessed 24 April 2025].
Toxigon Infinite, 2025. Handling Multicollinearity in Regression Analysis: Practical Tips and Techniques - Toxigon. [online] Available at: <https://toxigon.com/handling-multicollinearity-in-regression-analysis?> [Accessed 25 April 2025].
under30ceo, 2024. Homoscedasticity - Under30CEO. [online] Available at: <https://www.under30ceo.com/terms/homoscedasticity/?utm_source=chatgpt.com> [Accessed 25 April 2025].

## License
The MIT License (MIT)

Copyright (c) 2025 Hannah Michaelson

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE




