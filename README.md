# covid_risk_tpu_regression
Investigating the Relationship between the Geographic Variations and Incidence Risk of COVID-19 in Hong Kong

TPU_preprocessing: 
1. ignore the case with incomplete information
2. count number of cases in each TPU
3. count number of cases in each TPU according to gendar and different age range


ratio_preprocessing:
1. divide all features with population of the TPU to calculate the ratio of the feature over population
2. split all cases into three groups, local cases, imported cases and unknown cases. 
3. To be accurate, only consider the local cases as the source of community virus spread.
4. according to the assumption in 3., we take (local case number in a TPU)/(population of the TPU) as the incidence rate instead of (all cases number in the TPU)/(population of the TPU).

ratio_regression:
1. training and testing of five regression models 
2. the results of all models in form of diagrams
3. feature correlation analysis
