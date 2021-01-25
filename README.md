
# PISA 2012
## by Lukas Jakson

**Table of Contents**

- [1. Introduction](#introduction)
- [2. Structure of PISA2012 dataset](#structure-dataset)
- [3. Questions](#questions)
- [4. Summary](#summary)
- [5. Key Insights](#key-insights)

<a id="introduction"></a>

## 1. Introduction to PISA

**What Is PISA?**

The Program for International Student Assessment (PISA) is a system of international assessments
that allows countries to compare outcomes of learning as students near the end of compulsory
schooling. PISA core assessments measure the performance of 15-year-old students in mathematics,
science, and reading literacy every 3 years. Coordinated by the Organization for Economic
Cooperation and Development (OECD), PISA was first implemented in 2000 in 32 countries.
It has since grown to 65 education systems in 2012.

**What PISA Measures**

PISA’s goal is to assess students’ preparation for the challenges of life as young adults. PISA assesses
the application of knowledge in mathematics, science, and reading literacy to problems within a reallife context (OECD 1999). PISA does not focus explicitly on curricular outcomes and uses the term
“literacy” in each subject area to indicate its broad focus on the application of knowledge and skills.
For example, when assessing mathematics, PISA examines how well 15-year-old students can
understand, use, and reflect on mathematics for a variety of real-life problems and settings that
they may not encounter in the classroom. Scores on the PISA scales represent skill levels along a
continuum of literacy skills.
Each PISA data collection cycle assesses one of the three core subject areas in depth (considered the
major subject area), although all three core subjects are assessed in each cycle (the other two subjects
are considered minor subject areas for that assessment year). Assessing all three subjects every 3 years
allows countries to have a consistent source of achievement data in each of the three subjects, while
rotating one area as the primary focus over the years. Mathematics was the major subject area in
2012, as it was in 2003, since each subject is a major subject area once every three cycles. In 2012,
mathematics, science, and reading literacy were assessed primarily through a paper-and-pencil
assessment, and problem solving was administered via a computer-based assessment. In addition to
these core assessments, education systems could participate in optional paper-based financial literacy
and computer-based mathematics and reading assessments. The United States participated in these
optional assessments. Visit www.nces.ed.gov/surveys/pisa for more information on the PISA
assessments, including information on how the assessments were designed and examples of
PISA questions.

Source: https://nces.ed.gov/pubs2014/2014024rev.pdf

<a id="structure-dataset"></a>
## 2. Structure of PISA2012 dataset

The original data set contains 485.490 students and 636 features. Therefore I looked in the dictionary to better understand the meaning of the variables. In the course of this, we found variables that will help us take a closer look at the following interesting features. 


<a id="summary"></a>
## 3. Summary of Findings

I wanted to find out if gender, migration background, and the country where the students wrote the tests had an impact on the scores, so I asked the following questions:

1. How do students compare globally in literacy performance in math, science, reading and overall?
2. Is there a difference in gender in terms of points scored?
3. Are there countries where students perform particularly well (99th percentile)?
4. Does a migration background have an effect on the points scored?

### 3.1. Univariate Exploration

Here we found that the genders were almost evenly distributed. Around one in eight of them had a migration background. Asian countries have the most students who are among the top 1%. In particular, Asian countries are dominant in mathematics. We also found that the proportion of girls decreases the higher the scores. 

### 3.2. Bivariate Exploration

Here we found that Asian countries consistently perform better than other countries. This means that it was probably not a case of outliers, but that this speaks for a consistently high level of education. In terms of migration, we were unable to identify any differences in the global average.  

### 3.3. Multivariate Exploration

We found that there is a strong correlation between the points scored and the subjects. This confirms our assumption that students who are good in one subject are also good in the other two. 

We were able to determine that the migration background in Germany does make a difference. We compared Germany with the USA, Israel, Canada, New Zealand and Australia. We saw that migrants of Turkish origin perform worse than migrants with roots in Poland or the former USSR. 

## 4. Key Insights

To see if gender plays a role in higher scores, we used a pie chart, outputting the 75th, 95th, and 99th percentiles. 

Because we wanted to know which countries were among the best, we used a bar chart to output the number of best 1% of students, but limited this to 20 countries. To check whether these are deviations, we output the score distribution of all countries using a boxplot.
In doing so, we found that the countries scored approximately the same points in each of the different disciplines. (NOTE to reviewer: This slideshow tool is not able to display the plotted graphics completely and when I make them smaller, they become unreadable. I have a degree in media design and use either InDesign for print stuff or online Tableau for storytelling.)

To check whether there is a correlation between the disciplines, i.e. whether students perform roughly equally well in all disciplines, we checked this with a pair plot. 

Finally, we wanted to see if the migration background had an effect on the points scored. To do this, we compared the classic immigration countries with Germany using a boxplot. 
