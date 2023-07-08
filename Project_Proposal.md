# Project Proposal

## 1. Motivation 
    
In the sight of the latest economic recession and layoffs in 2023 from top big tech companies, it has become mayhem in the tech industry. Candidates aspiring to get rehired are facing uphill battles with the competition in the market. Though many sectors (i.e, Banking, Health, Mining, Automobiles, etc. ) have the same jobs and requirements, the job titles vary a lot representing the sectors from which the job arises. Our annotated corpus of Job titles and skill sets will help job seekers move across sectors for jobs with right skills.

## 2. Source and structure of the data

In this we are working on job descriptions from LinkedIn jobs and Indeed.
We are restricting our job titles to Tech Industry as all the team members are from tech background.

We are scrapping any data job description that is looking arising out of Canada and Tech Industry.

**Structure of the data**

A Job description consists of around 1000 tokens (words). We are planning to scrap from LinkedIn and Indeed job postings.
Most of the time the text are English and sometimes in French, but here for our annotating we are trying to go ahead with English. Most job descriptions and roles don't have a defined structure, as they are written according to the Recruiter's preferences.
Mostly we might have broad classifications on requirements and qualifications in most of the Job descriptions.


## 3. A preliminary annotation 

### 3.1 Annotating job titles

We are looking to Annotate the following :

1) `SKILLS` - Technologies paraphrased from the job description. eg: Python, Java, Agile, Scrum, etc.

2) `CLASS_NAME`  - job title (not the job title from LinkedIn). eg: Data Scientist, Quality Analyst, Front-end developer, etc.

3) `EXPERIENCE` - Experience level required for the job. example: Novice, intermediate, Advanced, Expert.


## 4. POC: A plan on building corpus of Job description and the skills serving them

We have written a python script to scrape the LinkedIn (jobs)/Indeed job posting for enough jobs so that we get around 1M+ tokens for our corpus to help the Job seekers.

## 5. Storing and Accessing data:

We are planning to use JSON structure, most of the job roles have multiple skills so an NO-SQL is a good approach.

## 6. Usage Metrics:

If the Corpus goes live we might be able to help job seekers in following ways:

* Can help job seekers look into cross sector jobs.
* Top skills used to get into any job.
* Understand most trending skills in job market.
