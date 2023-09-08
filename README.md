# Thermal conductivity of Oxides
**Note:**<br>
This is part of an introductory class to Material Informatics. Kindly go through the pdf of the presentation to check if this is relevant to your work. All three of us had no prior knowledge of Machine Learning. For creation of the project we utilized the following steps:

### Data Collection:
We used Matminer to extract properties for oxides from AFLOW database. Oxides were chosen for their relative low thermal conductivity.

### Data Filtration
We did a Principal Component Analysis (PCA) to ensure overfitting was avoided. Also plotted a pie chart that helped remove outlier oxides. (Bravais Lattices that were less than 2% of the total number of oxides). Heat maps validated the PCA results.  

### Deep Neural Networks
80% of the data was taken for training the model and 15% for validation. Remaining was used as test case. 
Used a feed forward deep neural networks with 4 layers and compared results from ADAM and RMSProp optimizers. Obtained a R2 score of 0.99 in each case. 
Subsequently studied the impact of features that gave such a high R2 score. Finally extended the study for nitrides and sulphides. Due to most oxides having low thermal conductivity, model is reliable for low thermal conductivity materials.
