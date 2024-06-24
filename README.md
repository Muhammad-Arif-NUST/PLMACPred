# PLMACPred

PLMACPred: Prediction of Anticancer Peptides based on Protein Language Model and Wavelet Denoising Transformation

##Pipeline

###PLMACPred uses the following dependencies:

MATLAB2018a *blast-2.6.0+
python 3.9
numpy
scipy 
pandas
scikit-learn
fair-esm==2.0.0
joblib

gc_forset *xgboost-1.5.0

###Guiding principles:

**The Dataset contain training dataset and testing dataset. ACP740 include ACP_740tr and TACP_740ts files. ACPMain include ACPMain_tr and ACPMain_ts files. ACPAlternate include ACPAlter_tr and ACPAlter_ts files in fasta format. 

**Feature extraction: CPSR is the implementation of component protein sequence representation. HOG-PSSM cantain PSI-BLAST file and HOG (histogram of oriented gradient )descriptor to convert the extracted PSSM into (HOG-PSSM), ESM2 and Prot5 are the pre-trained modles

** Classifier: PLMACPred.py is the implementation of proposed method, SVM.py and NB.py to predict ACP and Non-ACP activities.
