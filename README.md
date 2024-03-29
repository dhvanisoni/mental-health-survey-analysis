# survey-analysis
This dataset is from a 2014 survey that measures attitudes towards mental health and frequency of mental health disorders in the tech workplace. 
There are a total of 26 columns and 1259 entries in the dataset. 

**Data Cleaning:**

In dataset four columns has null values - state (515), self_employed (18), work_interfere (264), comments (1095)

we will drop the timestamp column because it's contains date, month, year and time the respondent took this questionnaire, which is irrelevant for us.
Comment column seems to contain most number ( 70% ) of null values, which makes sense because it was an optional text box so it's reasonable to expect that many (most) respondents would leave it blank.

So, drop columns from datasets that are not useful. drop timestamp and comments and create new dataframe.

The state column also contains a lot of null values. We'll not need that column also.
we have state columns only for United states 

Handle missing values in self_employed column and work_interfere column by filling null values.

Create new_df and keep only relevent columns which are useful in our analysis.
(Age, Gender, Country, remote_work, self_employed, tech_company, 
phys_health_interview, mental_health_interview, mental_health_consequence, phys_health_consequence, family_history, treatment, benefits, wellness_program)

Reason for selecting  these variables:
Mentle illness is very relevent to person's age, gender and work. 
Sometimes it depends on person's work, whether he/she is working in remotely or in workplace,whether he/she is self-employes or not, whether he/she working in tech-company or not.
Family history also play major role in mentle disorder.

**Problems that I have encountered:**

Gender columns have so many categories so , I have grouped them into three categories like Male, Female and Other.

Age column have some incorrect values so I dropped them and grouped remaining values into four categories - under 18, mid age , young age ,old age

I consider Maybe as Yes in mentle and physical health columns because when respondents says maybe which means they have some symptoms of mental health illness.

Most respondents are from United States, United Kingdom and Canada and others countries have less 50 repondents
and some countires have 1 or 2 respondents that are not useful in for analysis.So, categorised counties in 5 different continents.

**Insights from Data Analysis:**

Survey conducted in total 48 counties. Most respondents are from United States, United Kingdom and Canada.

People who are self employed and people who are not self employed they both need treatment.
We can say that whether a person is self employed or not, does not largely affect whether he may be seeking mental treatment or not.

We can say from our analysis, most predominent gender group from survey respondents are male, followed by Female and Other.

Mental illness have found majorly in tech filed as most positive respondents are working in a tech company

Around 70% of respondents don't work remotely, which means the biggest factor of mental health disorder came up triggered on the workplace.
wheather people are working in tech and non-tech company, both need treatment.

Most of the respondants employers haven't discussed mental health as a employee wellness program.
Companies should include mental health in the employee wellness program.This shouldn't be overlooked

Most respondents do not have family history but they need treatments. In United States more people seeking for treatment compare to other nations.

**How does the frequency of mental health illness and attitudes towards mental health vary by geographic location:**

Mental health illness effects diffenrently in different geographic location. Most people are having mental illness and seeking for treatment is in United States,but in European 
country and Asian country most respondents do not need treatment for mental health illness. In Oceania  and African countries most people have mental illness and seeking treatment  for mental helath illness 

Most people having mental illness are working in a tech company and majority of them belongs to young age group and are male.
