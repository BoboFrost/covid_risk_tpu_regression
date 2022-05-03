# covid_risk_tpu_regression
Investigating the Relationship between the Geographic Variations and Incidence Risk of COVID-19 in Hong Kong

TPU_preprocessing: 
1. Ignore the case with incomplete information
2. Count number of cases in each TPU
3. Count number of cases in each TPU according to gendar and different age range


ratio_preprocessing:
1. Divide all features with population of the TPU to calculate the ratio of the feature over population
2. Split all cases into three groups, local cases, imported cases and unknown cases. 
3. To be accurate, only consider the local cases as the source of community virus spread.
4. According to the assumption in 3., we take (local case number in a TPU)/(population of the TPU) as the incidence rate instead of (all cases number in the TPU)/(population of the TPU).

tpuFeatures_incidenceRate_regression:
1. Training and testing of five regression models 
2. The results of all models in form of diagrams
3. Feature correlation analysis
