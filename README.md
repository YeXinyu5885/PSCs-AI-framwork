# PSCs-AI-framwork
The database of the paper "A Universal Artificial Intelligence Framework for Multi-Scale Design and Optimization of Perovskite Solar Cells."
1) System requirements
# Operating system
MacOS Mojave (10.14.6)

# Programming language
python (3.7.4)

# Required python libraries:
pandas (0.25.1)
numpy (1.17.2)
sklearn (0.21.3)
pycm (2.5)

2) Installation guide
Install python and the above mentioned python libraries using pip or conda. No other specific installation is required. Typical install time for the above python dependencies is around 5 minutes.

3) Demo
Five python scripts are included to generate error statistics (classification error metrics for training and test sets as a function of training set size) to plot Figure 3 in the main manuscript, and make predictions on the validation set of 10 MOFs and for new 88 MOFs. Using the terminal, the following commands should be given to execute the python scripts.

# Script to create learning curves for SVM, RF and GB models for the case of 2-class models
python svm_rf_gb_2class.py

# Script to create learning curves for SVM, RF and GB models for the case of 3-class models 
python svm_rf_gb_3class.py

# Script to create learning curves for RF model with all features. For comparison with RFE-based feature models 
python rf_all_features.py 

# Script to make predictions on validation/new set of MOFs using pre-trained 2-class model
python prediction_2class.py

# Script to make predictions on validation/new set of MOFs using pre-trained 3-class model
python prediction_3class.py


Expected run time is around 1 hour for each of the first three scripts, while later two should be complete in less than a minute.
