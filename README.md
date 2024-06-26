## Objective

As part of the Business Intelligence Systems Infrastructure program curriculum at Algonquin College, Ottawa campus, our team was provided the opportunity to carry out a capstone project sponsored by Health Canada and Mr. Chris Thompson. 

The opportunity presented to the team was to leverage our skills gained from the program to achieve the following objectives:

1.  Explore the public service employee survey results for employees working in Health Canada and the Public Health Agency of Canada and conduct a sentiment analysis.

-  Collect data from the open datasets on the federal service portals about Health Canada and the Public Health Agency of Canada.

-  Analyze the data to find out the sentiment using a score out of 5, based on themes, subthemes, demographics, and questions.

2.  Develop interactive dashboards that show sentiment trends over time as well as differences and similarities between Health Canada and PHAC and for employee demographic groups.

-  Showcase a story through interactive and dynamic dashboards.

-  Identify historical trends.

-  Compare different groups and demographics.

3.  Focus on learning and define technical aspects to meet program expectations.

-  Complete all deliverables assigned in class including reports/presentations.

-  Utilizing tools such as Power BI and Excel along with leveraging all the skills gained throughout this program. 

## Logical solution

Our logical solution involved the following steps:

## Data Collection

We collected the PSES survey results from the open datasets on the federal service portals about Health Canada and the Public Health Agency of Canada.

## Data Exploration

We went over the data to understand what each column represented and the function it would serve towards us getting the correct sentiment.

Our datasets included the following demographic categories:

●  How long people have worked there?

●  Their age.

●  If they're supervisors.

●  Their gender.

●  2SLGBTQIA+ status.

●  Ethnic diversity categories.

●  The region in which they work, 

●  Their first language.

●  If they work in bilingual roles.

The main themes or organizational dynamics considered were:

●  Employee engagement

●  Leadership

●  Workforce

●  Workplace 

●  Workplace well-being

●  Compensation

## Data Preparation

We cleaned the collected data using Microsoft Excel by filtering out the data that we deemed not useful in our analysis such as French-written columns, suppressed data, various survey questions, and blank rows. 

We also categorized each question in the survey that did not have a calculated sentiment score out of 5 calculated, as either positive or negatively coded to help us derive the sentiment in later stages.

## Data Preprocessing

To satisfy the client's requirement to include keywords in our sentiment analysis, we preprocessed the question data, by using a Python algorithm to remove noise such as punctuation, stop words, and special characters.

## Feature Engineering

From the preprocessed questions data, we derived a new column with keywords for each entry in the datasets.

To calculate a sentiment score out of 5 for each entry with a missing score, we used the aggregated result of the agree column and the type of question, positively or negatively coded, to derive the score.

## Sentiment Analysis

We derived the overall sentiment for each entry based on the calculated score out of 5.

To categorize the sentiment, we used the range below:

-  Less than 2.5 = Negative

-  2.5 to 3.4 = Neutral

-  Greater than or equal to 3.5 = Positive

We further calculated the average sentiment score for each question using DAX measures and categorized the sentiment based on the range above. 

## Digital Solution

Our digital solution was to leverage Microsoft Power BI to visualize the results of the sentiment analysis and showcase a story through interactive and dynamic dashboards which would help us identify historical trends and compare different groups and demographics.

## Interactive Dashboards

Using Power BI, we designed interactive dashboards that allowed users to explore sentiment analysis results. Users could filter data based on various parameters, such as survey years, themes, subthemes, and demographic groups.

## Dynamic Visualizations

The dashboards featured dynamic visualizations, including trend charts, word clouds, and sentiment distribution plots. These visualizations enabled the client to gain deeper insights into sentiment patterns and trends.

## Storytelling through Data

Our approach emphasized storytelling through data visualization, where each dashboard conveyed a compelling narrative. By presenting data coherently and engagingly, we aimed to facilitate understanding and decision-making.

Elaboration on results and analysis

Some of the key findings from the analysis were:

●  The sentiment analysis was averagely positive with a score of 3.58.

●  The results showed that employees did not feel discriminated against, with the topic having the highest sentiment score (4.45)

●  People with experience of less than 3 years in the federal service had the highest positive sentiment.

●  People in the National Capital Region had the highest positive sentiment when regions were considered.

●  The average sentiment score dropped from 3.66 in 2019  to 3.54 in 2022. Potential reasons for the decline could be due to suppressed data in the years before 2022 or external factors such as COVID-19 and inflation.

●  Health Canada and PHAC both had an overall average positive sentiment with Health Canada having a slightly higher percentage 68% compared to PHAC's 65%.

●  Employees in Health Canada had a slightly higher sentiment score 3.01 compared to their colleagues in PHAC 2.97 when asked about compensation.

●  The sentiment score for the Workplace well-being theme took a 0.1 dip from 3.89 to 3.79 between 2019 and 2020. Which was the lowest in all the years the survey was taken.

●  2SLGBTQIA+ Transgender people had a low sentiment score (2.36), specifically about the duty to accommodate them and their workplace being psychologically healthy.

## Proposed data story

We developed three dashboards that aimed to tell a story about our findings. 

## The Main Dashboard.

The main dashboard was meant to visualize the overall sentiment score, the change of sentiment over time, the top five demographics with positive and negative sentiments, the top five themes with positive and negative sentiments, and the keywords associated with positive or negative sentiments. 

![alt text](ONE.PNG)

The dashboard allows the user to drill down by organization, demographic, survey year or theme using slicers.

## The Question Analysis Dashboard

![alt text](TWO.PNG)

This dashboard aimed to drill down on each question from the survey, survey, organization and demographics. From this dashboard, you would find out the average sentiment for each question and sub theme based on the organization or demographic.

## The Sensitive Demographic Comparison Dashboard

This dashboard was meant to compare the sentiment and sentiment change over time for the demographics we considered as the most sensitive, which were gender, racial diversity, and the 2SLGBTQIA+ status. The user can drill down by organization and sub-theme using slicers.

![alt text](THREE.PNG)

## Value

This solution provided valuable insights to enhance the workplace environment and employee satisfaction within these government agencies based on organizational dynamics, workplace culture, and demographic groups.

It also enables the agencies to compare how different demographic groups currently feel toward various aspects of the organization.

## Cautions

Since we calculated the sentiment based on the average score out of 5 per demographic, question, theme, or subtheme, some categories with a low answer count could lead to unusual ranking.

## Lesson learned

The main lessons learned included:

●  The importance of involving stakeholders early and throughout in the business intelligence project development process, 

●  The value of iterative development and feedback loops

●  The best practices for data cleaning, preprocessing and analysis.

●  Strategies for effectively communicating insights to technical and non-technical audiences.

●  Working cohesively and effectively as a team to achieve the desired result.

## Features we wish we had implemented

●  An additional layer of categorization of the questions based on the keywords.

Due to insufficient results from various NLP models, we could not come up with an extra layer of categorization for the question which would have supplemented the themes and sub-themes in our datasets.

## Conclusion

After a fruitful three months of working as a team, we achieved our objective of exploring the public service employee survey results for Health Canada and the Public Health Agency of Canada, conducting sentiment analysis, and developing interactive dashboards to showcase trends and insights.

The key findings revealed an overall positive sentiment among employees, with certain demographic groups and themes showing variations. Opportunities for improvement were identified, including the need for better data description, accommodations for the transgender community, and strategies to reduce work-related stress and increase employee engagement. 

As we reflect on our accomplishments, we take pride in our collective efforts and the impactful insights we discovered. We look forward to developing more data-driven solutions by utilizing the skills we have gained from this program.
