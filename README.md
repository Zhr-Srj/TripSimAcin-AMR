# TripSimAcin-AMR
A deep learning-based framework for predicting antimicrobial resistence phenotype in Acinetobacter Baumannii bacteria.

## Code folder
Consists of all ipython notebook files used to get the results mentioned in the article:
* SHAP_Analysis.ipynb:
  - Is used to conduct SHAP analysis to identify the most important features.
  - Includes the results mentioned in Table 2 and Table 3 in article.
* TripSimAcin_AMR_validation1.ipynb:
  - 10 times validating TSA-Net and TripSimAcin-AMR framework.
  - Includes contents of Table 4 and Table 5 in article.
* TripSimAcin_AMR_validation2.ipynb:
  - 10 times validating performance of TSA-Net and TripSimAcin-AMR on external dataset.
  - Encompasses the results of Table 7 and Table 8.
* TripSimAcin_AMR_validation3.ipynb:
  - Comparison of TripSimAcin-AMR with traditional machine learning models was done in it.
  - Results are mentioned in Table 6.
* TripSimAcin_AMR_PerDrug.ipynb:
  - Assessing TripSimAcin-AMR's performance, predicting AMR phenotype for each of the mentioned antibiotics, on external dataset.
  - Figure 5 in the article was made in this file.
* LRcomparison.ipynb:
  - Comparison of Logistic Regression performance with other baseline models.
  - Table 9 contents are from this file.

## Data folder
Includes all datasets used in the article's analysis.
* Dataset19.zip:
  - Input file for SHAP_analysis.ipynb.
  - Each line corresponds to a strain-antibiotic pair.
  - Each line is strain's feature vector followed by antibiotic's feature vector.
* drugLabel19.txt:
  - Includes corresponding pair's antibiotic name and resistance phenotype.
  - 1 indicating "Resistant" phenotype and 0 indicating "Susceptible"
* Dataset_SHAP_u.zip:
  - Dataset19.txt after feature reduction using SHAP.
* DrugLabel_SHAP_u.txt:
  - Includes antibiotic names and resistance phenotypes of pairs according to Dataset_SHAP_u.zip file
* Strain_aside_Dataset_SHAP.txt:
  - The external dataset mentioned in article.
  - Each line corresponds to a strain-antibiotic pair.
  - Each line is strain's feature vector followed by antibiotic's.
* Strain_aside_drugLabel_SHAP.txt:
  - Each line corresponds to the same line in Strain_aside_Dataset_SHAP.txt file.
  - Each line encompasses the antibiotic's name followed by resistance phenotype of the strain to this antibiotic.
  - 1 indicating "Resistant", while 0 indicates "Susceptible".
  
