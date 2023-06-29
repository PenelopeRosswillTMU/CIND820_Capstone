# CIND820_Capstone

## Tentative stages of the project: 
  - Problem solve ways of combining the blocks into one dataset without making the file too large (done - keep in blocks, but add description to rationale)
  - re run analyses with combined dataset (done - no longer necessary)
  - see what additional feature selection tools are available for categorical datasets 
  - decide which variables are best to use for modelling and answering research questions (done - see below)
  - run all analyses using the decided variables
  - Create confusion matrix for the classification methods used
  - create presentation documents 

## Repository Guide
  - EDA HTML Reports: the reports generated based on the complete dataset "EDA Report.HTML", and then the 4 blocks of data created to make the multiple selection id duplication manageable "EDA Report_block1-5.HTML"
  - the original dataset from the survey and the 4 separated blocks, in csv format.
  - ipynb files for the EDA reports and code for the feature selection on block 1 (chi squared and mutual information)
  - results of the feature selection process
  - table of the accuracy scores for each variable that would potentially be used as output variables from block 1

## Research Questions
-	What intersections of identity impact LGBTQ+ Canadians need and use of social services? 
-	Do the intersections of identity correlate with specific use of social services? 
-	How does physical location in relation to the centers offering social services impact participation?
-	Does the success of a certain social program vary on the identity of the person using them? 
-	Does income and education affect the use of social services?

## Features Decided on 
  Feature Selection was based on the Chi Squared Test done on each block of data (4 blocks plus 1 block for participant identity information). The top 5 scores were counted for each block. Features 1-5 listed below were from the identification block, Feature 6 was from block 1 (Access to City of Montreal services), Features 7-9 were from block 2 (Environmental and Quality of Life), and Features 10 and 11 were from block 3 (Security in a Public Space). No features were selected from block 5. <br> <br>
  Dependant Variable: 'Do you identify as a trans person, or have you had a trans background at some point in your life?' <br>
  Features:
  1. 'How many years have you lived in Montreal?'
  2. 'What age group are you in?'
  3. 'How do you identify yourself?'
  4. 'What is your sexual orientation?'
  5. 'Are you a member of a First Nation or Inuit Nation?'
  6. 'Do you agree with this statement: “in general, the services of the Ville de Montréal meet my needs”?'
  7. 'Do you agree with this statement: “in general, I feel comfortable being myself in my daily activities in Montreal”?'
  8. 'In the past two years, have you experienced unfavorable or differential treatment because of your gender identity and expression or your sexual orientation? Check all that apply. Please note that some of these services are offered by parties other than the Ville de Montréal.'
  9. 'Give your level of agreement with each of the following statements regarding the Montreal reality. Please note that some of these services are not offered by the City of Montreal.'
  10. 'In the past two years, have you experienced any of the following behaviors because of your gender identity and expression or sexual orientation? Check all that apply.'
  11. 'If you did not file a complaint, why? Check all that apply.'
