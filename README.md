# README file for the dissertation project titled " Machine learning and statistical approaches for the diagnosis of schizophrenia using molecular markers"

Aim: To compare the class prediction abilities of the support vector machine-radial (SVM-rad) and logistic regression (LR) for disease classification of SCZ. 

Data type: Microarray gene expression data from publicly available platform

Packages used: Refer the scripts

About the script
The gene expression data was processed and used for model comparison using the scripts shared. The numbers before the title of the script indicate the sequence in which analysis was performed. Below are the details of the analysis:

1. Data processing and annotation: The gene expression data was processed with respect to the different platforms and annotated with the help HGNC nomenclature.

2. Creating metafile: A metafile was created that contained the processed datasets combined on the basis of the common feature genes.

3-6. Analysis with the variable numbe of sample observations and feature genes

  1. Training and Testing data: The script includes shuffling and random sampling of the train and the test data.

  2. Quantile normalization: Training data was independently quantile normalized and the saved targets from each dataset was used for test data normalization in reference to the train data.

  3. Batch correction: The train data was batch corrected using ComBat to remove the technical difference between the different batches. The test data was batch corrected in reference to the train data. 

  4. Feature selection: Feature selection was performed using Differential gene expression analysis. Feature genes identified from each train data was used to build the LR and SVM models.

  5. Building LR and 6. SVM models: Models were built using the different sample observatio and feature gene subsets. Models were tested using test datasets. Models and test data predictions were saved for further analysis. 


Contact:
Tanvi: tanvi.kottat@ssbs.edu.in
