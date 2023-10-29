## Project Overview

Annually, the FSB conducts a senior survey of graduates to learn of their employment status.  In addition, information is verified using LinkedIn and employer survey information.  The data you are provided ('FSB_BI_Survey_2019_2021.rds') contains data on graduates for 2019, 2020, and 2021.  The data are merged from two sources:  the senior survey, and data from the Miami University database.  

The data are anonymized, however it is possible that if you look hard enough, you can identify students.  You are bound, ethically not to do so.  It is a strict ethical code that you will not discuss individual data points with ANYONE except for me and your team.  Failure to comply with this code of ethics will result in a failing grade in the course.  

## Business Value Proposition 

The product and service this analysis will provide is a soundbite on the geographic trends in FSB placement data. Our clients will utilize our insights to help drive business decisions. For example, Miami University may decide to target companies from a specific geographic area, based on salary or job type to bring to career fair for a specific major. The provided dataset is comprehensive with 42 different attributes per row. This analysis will provide our client with meaningful insights without having to process the dataset. This pain killer will allow our clients to focus their time at work in other areas. 

## Data Sources

You have three years of data representing FSB graduates, including graduates in 2019, 2020, and 2021.  The dataset provided had 42 variables.  The source is either derived by me during data cleaning/merging, from the Oracle Business Intelligence Enterprise Edition (OBIEE) maintained by Miami adminsitration, or from the self reported senior survey.  I have cleaned and merged the files into one file.  

1.  nmajor: numeric,derived, the number of majors 
2.  major1: text, OBIEE, first major
3.  major 2: text, OBIEE, second major
4.  BBRJ: binary, OBIEE, an attribute of a student, but we do not know what this stands for
5.  Business Direct Admit: binary, OBIEE, a direct admit to FSB as a first year
6.  Combined Cacc and Masters: binary, OBIEE, combined degree student
7.  Dean's List: binary, OBIEE, achieve dean's list status at least once
8.  First Generation College Stdnt: binary, OBIEE, first generation student status
9.  FSB Scholars: binary, OBIEE, FSB scholars program
10.  Honors Program: binary, OBIEE, member of University honors program
11.  President's list: binary, OBIEE, achieved president's list at least once
12.  Study Abroud Courtesy Account: binary, OBIEE, do not know meaning
13.  Transfer Work: binary, OBIEE, do not know exact meaning
14.  Cum Laude: binary, OBIEE, graduated Cum Laude
15.  Magna Cum Laude: binary, OBIEE, graduated Magna Cum Laude
16.  Summa Cum Laude: binary, OBIEE, graduated Summa Cum Laude
17.  University Honors: binary, OBIEE, graduated with University Honors
18.  University Honors w/Distinction: binary, OBIEE, graduated with University Honors with Distinction
19.  minor1: text, OBIEE, first listed minor
20.  minor2: text, OBIEE, second listed minor
21.  IPEDS.Race.Ethnicity: text, OBIEE, race/ethnicity
22.  Gender: text, OBIEE, sex
23.  GPA.Range: text, OBIEE, GPA within a .5 range
24.  Term.Code: numberic, OBIEE, First four digits are the physcal year (beginning in July, e.g. July 2020 is FY 2021).  Last two digits is the term (10=fall, 15=winter, 20=spring, 30=summer).
25.  Year.x: text, derived, first four digits of Term.Code stored as a character variable
26.  latin_honors: text, survey, latin honors designation
27.  survey_city: text, survey, student reported city in which their job is located
28.  survey_company: text, survey, student reported company in which they accepted a job
29.  survey_deptfunc: text, survey, student reported job function
30.  survey_gradprogram: text, survey, student reported graduate program they will be attending
31.  survey_gradschool: text, survey, stuent reported graduate school they will be attending
32.  survey_internfour: text, survey, student reported fourth internship they held during college
33.  survey_internthree: text, survey, student reported third internship they held during college
34.  survey_interntwo: text, survey, student reported second internship they held during college
35.  survey_internone: text, survey, student reported first internship they held during college
36.  Survey_internships: text, survey, Student reported number of internships they held during college
37.  survey_offers: text, survey, student reported number of offers for full time employment received
38.  survey_plans: text, survey, student reported plans after graduation
39.  survey_pref_field: text, survey, student reported whether working in preferred field
40.  survey_pref_loc: text, survey, student reported whether working in preferred location
41.  survey_salary: numeric, survey, student reported salary
42.  survey_state: text, survey, student reported state in which job is located

## Process on Running the Data

This responsitory contains 2 rmd files.  The first FSB_Student_Geographic_Trend_Analysis and Flexdashboard.  Each file targets 2 separate things.  The first file is focused on cleaning the data and getting it ready for viziualizations.  The second file is the dashboard with the vizualizations for the taget question.  In order to produce the same results, run the FSB_Student_Geographic_Trend_Analysis.rmd file first to produce the output file that has the cleaned data.  Then run the Flexdashboard.rmd file to produce the dashaboard created.

## Deliverables

list of deliverables to the client and explanation of how each deliverable addresses their pains or needs. This analysis will address the pains and needs of our Client. Our client wishes analyze the geographic trends of the FSB student success data while also considering and controlling on outside factors such as salary, internships, and major. To address this our report will first clean the data. This cleaned data set is one of the products that we will provide our customers as it allows for ease in future analyses. Then this clean data will be intuitively used to create a comprehensive dashboard to address the clients specific questions.
1. The first page will provide graphics on top placement locations from FSB students. There will be a visual dot plot map focusing on placements within the US, as well as a table of the top ten placement locations by city (including count). This will address the clients question regarding where FSB students are going.
2. The second page of the dashboard will explore the salary differentials between states as well as the average salaries of placements within the top 10 most placed in cities. This page will address the client’s interest in exploring the salary differentials by region.
3. The third page of the dashboard will provide tables and statistics to describe the types of jobs students are getting per region, as per our clients request. Additionally, it will provide the types of jobs by city for both NYC and Chicago.
4. The fourth and final page of our dashboard will provide the top company employment counts for FSB students by the four cities (Chicago, Cincinnati, Cleveland and Columbus). This addresses our clients question about the top jobs by city for the “4 C’s”
