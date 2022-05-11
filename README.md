#   UTIVA  Power-BI-Capstone-project
# Case Study: HR Analytics to analyse the company’s HR data and come up with recommendations for management’s attention.
Role: Human Resource Analyst

Target Audience: Management

Tool(s) used: Microsoft Power BI

### Introductiion
The Palmoria Group, a manufacturing company based in the Nigeria is 
embroiled in issues bordering on gender inequality in its 3 regions. 
Unfortunately, the media recently published in the news with the 
headline “Palmoria, the Manufacturing Patriarchy” This doesn’t look 
good for the owners of the business based on their ambition to scale 
the business to other regions and even overseas. Cases like this can 
only spiral downwards revealing other issues like gender pay gap 
amongst other possible issues.
The CEO of Palmoria, Mr Ayodeji Chukwuma is keen to address these 
issues before it gets out of hands. The CHRO, Mr. Yunus Shofoluwe has 
been assigned the task to identify key areas within the business that 
could spring up issues and address them immediately

## The Business Solution

### For this case study my final report in Power BI will make the  Management make their decisions by evaluating the following ;

1. What is the gender distribution in the organization? Distil to 
regions and departments

2. Show insights on ratings based on gender

3. Analyse the company’s salary structure. Identify if there is a 
gender pay gap. If there is, identify the department and 
regions that should be the focus of management

4. A recent regulation was adopted which requires 
manufacturing companies to pay employees a minimum of 
$90,000
- Does Palmoria meet this requirement?
- Show pay distribution of employees grouped by a band of 
$10,000. For example: How many employees fall into a band of 
$10,000 – $20,000, $20,000 – $30,000 etc. Also visualize this 
by regions

5. Mr Gamma thought to himself that since you were already working 
on the employee data, you could help out with allocating the annual 
bonus pay to employees based on the performance rating. He handed 
another data to you that contains rules for making bonus payments 
and asked you to
- calculate the amount to be paid as bonus to individual 
employees
- Calculate the total amount to be paid to individual employees 
(salary inclusive of bonus)
- Total amount to be paid out per region and company-wide

## THE APPROACH
I followed this approach in modelling the solution above for the business challenge:

![1_hAuqn2Ap4bfpuPOZfHKO_w](https://user-images.githubusercontent.com/96060060/167625450-342e6109-fb26-4a89-a0ef-3dd05263d4f1.png)

## BUSINESS UNDERSTANDING

To give an accurate solution to the Business problem, you need to have proper understanding of the the business.it creates a road-map for moving forward, framing the business problem and proffering effective business solutions.

### *The main goal of this cas study is to help the Palmoria group to know whether there are gender related issues within the organization and its regions*

In order to communicate effectively with management so action can be made based on the insights generated there is need to leverage on business intelligence applications. For this business case I leveraged on Microsoft Power BI for my data analysis and visualization.

## DATA UNDERSTANDING

## A Microsoft Excel Worksheet (.xlsx) dataset was provided for analysis consisting of 1016 rows and 6 columns

The Palmoria Data workbook consist of the Name, Gender, Department, Salary, Location and Rating

An overview of the datasets are shown below;

![Screenshot (94)](https://user-images.githubusercontent.com/96060060/167632149-80210450-9ba1-4914-b1ae-afd423ddfb2b.png)

From the overview of datasets displayed above, it’s important and necessary we prepare the datasets before analysis and visualization is carried out.

## DATA PREPARATION
In preparing the data the first step taken was to Prepare the Excel workbook, ensuring the Excel file was shapened as seen in the figures displayed above, what this means is i  converted the data(columns & rows) to Standard Excel table format.

This was to ensure only the required table needed for analysis is loaded into PowerBi, If the workbook is not prepared in this way PowerBI will just ignore it and give you  a wrong results.

The next step I took was to extract my already formatted Excel workbook into PowerBI and load into Power Query Editor for proper data preparation.

## Data Prep in Power Query

The Power query tool in Power BI is used to get and transform data for appropriate analysis. Upon clicking Transform Data and navigating to power query window, I explored the data composition in order to know if any necessary data cleaning is needed by leveraging the Data Profiling Distributor feature which gives a summary of the column quality, distribution and profile.

While exploring the data I discovered that there were some empty spaces in the the Gender and Salary column. So in the Gender Column I replaced those empty spaces with 'Undisclosed' while in the Salary column I replaced the empty spaces with 'Null'. I also ensured the data type was in the right format for each column as it is imperative to be able to analyze effectively and generate accurate result.

![Screenshot (95)](https://user-images.githubusercontent.com/96060060/167920682-13634874-0596-4af7-a3b8-5ddd0af19809.png)

## DATA ANALYSIS
In other to answer the key questions needed to make the business decision there is need to analyze the data provided to gain insights which will then be visualized to effectively communicate to management.

The first thing I did in extracting insights from the data provided was to use a Data Analysis Expression(DAX) in creating a salary band for the employees to know each employee's salary band. i achieved this result by using the 'SWITCH COMMAND'. 

![Screenshot (96)](https://user-images.githubusercontent.com/96060060/167950544-26f4ef10-b9a7-4a6d-991a-e47259f8aaeb.png)

The second thing I did with the Data Analysis Expression(DAX) was that i created a bonus percentage column for each of the rating amd for each department by using the the 'if' command

![Screenshot (96)](https://user-images.githubusercontent.com/96060060/167950835-b0c63209-79c5-42b2-b68f-baca6591f034.png)

I also created a column which contains amount to be paid as bonus to the employees. I got that by multiplying the bonus percentage by the salary

![Screenshot (99)](https://user-images.githubusercontent.com/96060060/167951293-12105f5c-fcb8-4d1c-be15-88c62c96ea6a.png)

In addition I also got the toatal salary paid out by adding the bonus per employee with the the salary

![Screenshot (100)](https://user-images.githubusercontent.com/96060060/167951374-f5989536-edc4-4b61-86c8-b8fd5fad00e4.png)


## Insights from the analysis
In order for management to make the best decision has know whether there are  gender related issues within the organization and its region I have summarized below some key insights which will guide management in the next step to take.

### 1 The Gender Distribution by Region and Department

The total male Employees in Lagos is 124 while the female Employees is 118

In Abuja, total male Employees is 159 while the female Employees is 158

In Kaduna, total male Employees 182 while the female Employees is 165

![Screenshot (102)](https://user-images.githubusercontent.com/96060060/167954976-53fefa0e-40b8-4ac4-923c-035d27961ce4.png)

 2  Insights on ratings based on gender

![Screenshot (101)](https://user-images.githubusercontent.com/96060060/167955345-d904e05c-d082-4d5c-8be5-285ae17505e9.png)

 3 Gender pay Gap

![Screenshot (103)](https://user-images.githubusercontent.com/96060060/167955911-6ff976d4-9174-4942-a254-7883b53aa5eb.png)

 Minimum pay: The mimimum pay in Palmoria company is $28000 which means the company does not meet the minimum pay rule set for manufacturing Company.
 Below is the pay distribution of each employee

![image](https://user-images.githubusercontent.com/96060060/167956648-b748f886-e7ec-4a79-ad7c-3b26a184697c.png)

The bonus paid  to each individual employee, total amount paid to individual employees (salary inclusive of bonus) and total amount to be paid out per region and company-wide is shown below

![Screenshot (105)](https://user-images.githubusercontent.com/96060060/167957536-dfae6490-4219-423b-a5a6-bd248ab2f3b0.png)


## DATA VISUALIZATION
I created a data visualization to  communicate effectively this insights generated to the management of pamoria company by taking into consideration the techniques and steps involved in data visualization.
To get the whole visualization of this report, check the file in the code folder of this Portfolio

## CONCLUSION
The insights derived have been able to answer key questions that will guide management in taking action to meet the set objective of the business.



