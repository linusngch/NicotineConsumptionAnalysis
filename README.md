# Nicotine Consumption Analysis Through Machine Learning

Link to data: https://archive.ics.uci.edu/dataset/373/drug+consumption+quantified

Link to notebook: https://github.com/linusngch/NicotineConsumptionAnalysis/blob/main/Nicotine%20Consumption%20Analysis%20Research.ipynb

**Project Introduction**
Nicotine is one of the most addicting agents has been said to be as addictive as cocaine and heroin. This substance interacts with the nicotinic acetyl chline
receptors of the brain and sets of a chain reaction, stimulating a dopamine release. This stimulation results in rewarded mood elevation, euphoria and a heightened
sense of cognitive function.

However, nicotine's impact has significant negative side effects behind this immediate gratification. Studies have shown nicotine to be highly correlated with long-term
health problems such as insulin resistence, metabolic syndrome, and risk of diabetes. Addition to these effects, NAChRs by nicotine has also shown effects which are vital
for the initiation and dvelopment of cancer. 

**Main Goal**
This machine learning analysis aims to identify those who are most at risk to becoming addcited to nicotine and to highlight the features which may influence 
nicotine addiction. This analysis will uncover various factors that could potentially contribute to the onset of nicotine dependency and will help support groups
highlight individuals who are most at risk to being addicted to nicotine. Through this, there will be the potenitial mitigate the health problems and loss of
life associated with nicotine. 

**Data**
The data utilized from this project was from UCI's database and describes individuals based on their age, gender, use of drugs and more. Listed below are the user attributes 
of the data used:

1. ID: is a number of records in an original database. Cannot be related to participant. It can be used for reference only.
2. Age (Real) is the age of partparticipant
3. Gender: Male or Female
4. Education: level of education of participant
5. Country: country of origin of the participant
6. Ethnicity: ethnicity of participant
7. Nscore (Real) is NEO-FFI-R Neuroticism
8. Escore (Real) is NEO-FFI-R Extraversion
9. Oscore (Real) is NEO-FFI-R Openness to experience.
10. Ascore (Real) is NEO-FFI-R Agreeableness.
11. Cscore (Real) is NEO-FFI-R Conscientiousness.
12. Impulsive (Real) is impulsiveness measured by BIS-11
13. SS (Real) is sensation seeing measured by ImpSS
14. Alcohol: alcohol consumption
15. Amphet: amphetamines consumption
16. Amyl: nitrite consumption
17. Benzos: benzodiazepine consumption
18. Caff: caffeine consumption
19. Cannabis: marijuana consumption
20. Choc: chocolate consumption
21. Coke: cocaine consumption
22. Crack: crack cocaine consumption
23. Ecstasy: ecstasy consumption
24. Heroin: heroin consumption
25. Ketamine: ketamine consumption
26. Legalh: legal highs consumption
27. LSD: LSD consumption
28. Meth: methadone consumption
29. Mushroom: magic mushroom consumption
30. Nicotine: nicotine consumption
31. Semer: class of fictitious drug Semeron consumption (i.e. control)
32. VSA: class of volatile substance abuse consumption
33. Alcohol: alcohol consumption

Rating's for Drug Use:
1.  CL0 Never Used
2.  CL1 Used over a Decade Ago
3.  CL2 Used in Last Decade
4.  CL3 Used in Last Year 59
5.  CL4 Used in Last Month
6.  CL5 Used in Last Week
7.  CL6 Used in Last Day

**Methodology**
To prepare the data for modeling, the columns Semer and Chocolate were removed as one is a control and the other is not a drug. Null values were removed and drug
usage was encoded into numerical values. The nicotine column was separated from the data and changed into True/False values, indicating whether the person uses
nicotine or not. Baseline models of logistic regression, SVM, KNN, and decision tree classifiers were created and their hyperparameters were optimized and cross-
validated with its dataset.

**Findings**
After this fine tuning, the machine learning classifiers yielded higher accuracy scores in testing data and ROC/AUC scores. Without fine tuning, logistic regression yielded
the higest accuracy. After, decision tree classifiers yielded the highest score with an increase by 0.08 in test data score and 0.18 in ROC/AUC scores. Logistic 
regression barely showed any difference in scores before and after fine tuning, whereas SVM had an increase in scoring on the test data, but a drop in score for 
the ROC/AUC score.

The decision tree classifier and logistic regression classifier both yielded the highest scores in terms of performance metrics. Feature extraction on these two 
models showcased similar results. Cannabis was the leading factor in signifcant influence on whether or not a user smoked nicotine. This makes sense as both drugs
are a type of smoking habit, whereas many others are consumption or needle based. Decision trees showcased that Amphet and Age were the next two leading factors on
whether an individual uses nicotine. Logistic regression had cocaine and VSA as its following leading factors.

**Next Steps**
The result of this machine learning analysis can help officials and healthcare workers develop more precautionary steps to prevent nicotine consumption. Knowing the
strong influence factor that cannabis has could significantly enhance our understanding of the complex interactions between substance use and public health. By leveraging
the insights gained from this analysis, policymakers can tailor targeted interventions and educational campaigns to address the specific challenges posed by cannabis in
the context of nicotine addiction.

Furthermore, the identification of key patterns and risk factors through machine learning can contribute to the formulation of evidence-based strategies aimed at 
reducing the prevalence of nicotine consumption. This comprehensive approach involves not only addressing individual substance use but also considering the interconnected 
dynamics between different substances.


**Sources**
1. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4363846/
