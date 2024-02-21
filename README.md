# Practical Application Initial Findings

Link to data: https://archive.ics.uci.edu/dataset/373/drug+consumption+quantified
Link to notebook: https://github.com/linusngch/week20practicalapplication/blob/main/Capstone%20Project%20Initial%20Findings.ipynb

Nicotine is one of the most addicting agents has been said to be as addictive as cocaine and heroin. This substance interacts with the nicotinic acetyl chline
receptors and stimulates dopamine transmission. This stimulation results in mood elevation and apparent improvement in cognitive function. However, nicotine has 
significant negative side effects such as insulin resistence, metabolic syndrome, and risk of diabetes. NAChRs by nicotine has also shown effects which are vital
for the initiation and progression of cancer. 

This machine learning analysis aims to identify those who are most at risk to becoming addcited to nicotine and the features which may influence nicotine addiction.
The data utilized from this project was from UCI's database and describes individuals based on their age, gender, use of drugs and more. Listed below are the user attributes 
of the data used:

ID: is a number of records in an original database. Cannot be related to participant. It can be used for reference only.
Age (Real) is the age of partparticipant
Gender: Male or Female
Education: level of education of participant
Country: country of origin of the participant
Ethnicity: ethnicity of participant
Nscore (Real) is NEO-FFI-R Neuroticism
Escore (Real) is NEO-FFI-R Extraversion
Oscore (Real) is NEO-FFI-R Openness to experience.
Ascore (Real) is NEO-FFI-R Agreeableness.
Cscore (Real) is NEO-FFI-R Conscientiousness.
Impulsive (Real) is impulsiveness measured by BIS-11
SS (Real) is sensation seeing measured by ImpSS
Alcohol: alcohol consumption
Amphet: amphetamines consumption
Amyl: nitrite consumption
Benzos: benzodiazepine consumption
Caff: caffeine consumption
Cannabis: marijuana consumption
Choc: chocolate consumption
Coke: cocaine consumption
Crack: crack cocaine consumption
Ecstasy: ecstasy consumption
Heroin: heroin consumption
Ketamine: ketamine consumption
Legalh: legal highs consumption
LSD: LSD consumption
Meth: methadone consumption
Mushroom: magic mushroom consumption
Nicotine: nicotine consumption
Semer: class of fictitious drug Semeron consumption (i.e. control)
VSA: class of volatile substance abuse consumption
Alcohol: alcohol consumption
Rating's for Drug Use:

CL0 Never Used
CL1 Used over a Decade Ago
CL2 Used in Last Decade
CL3 Used in Last Year 59
CL4 Used in Last Month
CL5 Used in Last Week
CL6 Used in Last Day

This analysis

Fine tuning the machine learning classifiers yielded higher accuracy scores in testing data and ROC/AUC scores. Without fine tuning, logistic regression yielded
the higest accuracy. After, decision tree classifiers yielded the highest score with an increase by 0.08 in test data score and 0.18 in ROC/AUC scores. Logistic 
regression barely showed any difference in scores before and after fine tuning, whereas SVM had an increase in scoring on the test data, but a drop in score for 
the ROC/AUC score.

The decision tree classifier and logistic regression classifier both yielded the highest scores in terms of performance metrics. Feature extraction on these two 
models showcased similar results. Cannabis was the leading factor in signifcant influence on whether or not a user smoked nicotine. This makes sense as both drugs
are a type of smoking habit, whereas many others are consumption or needle based. Decision trees showcased that Amphet and Age were the next two leading factors on
whether an individual uses nicotine. Logistic regression had cocaine and VSA as its following leading factors.

The result of this machine learning analysis can help officials and healthcare workers develop more precautionary steps to prevent nicotine consumption. Knowing the
strong influence factor that cannabis has could significantly enhance our understanding of the complex interactions between substance use and public health. By leveraging
the insights gained from this analysis, policymakers can tailor targeted interventions and educational campaigns to address the specific challenges posed by cannabis in
the context of nicotine addiction.

Furthermore, the identification of key patterns and risk factors through machine learning can contribute to the formulation of evidence-based strategies aimed at 
reducing the prevalence of nicotine consumption. This comprehensive approach involves not only addressing individual substance use but also considering the interconnected 
dynamics between different substances.


Sources:
1. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4363846/
