# Thermal Conductivity of Oxides

**Note:**<br>
This repository is part of an introductory class on Material Informatics. Please review the PDF presentation to determine if this project is relevant to your work. We want to emphasize that all three of us had no prior knowledge of Machine Learning, and this project was created using the following steps:

## Overview

This project focuses on predicting the thermal conductivity of oxide materials, an important property for various applications in material science. We utilized a combination of data collection, filtration, and deep neural networks to achieve accurate results.

## Project Steps

### Data Collection

We obtained the necessary data by using Matminer to extract properties for a wide range of oxide materials from the AFLOW database. Oxides were chosen due to their relatively low thermal conductivity, making them an interesting subject for prediction.

### Data Filtration

To ensure the quality of our dataset and prevent overfitting, we implemented the following filtration techniques:

- **Principal Component Analysis (PCA):** We applied PCA to reduce the dimensionality of our dataset while preserving important information. This helped prevent overfitting and improved the model's generalization.

- **Outlier Removal:** We generated a pie chart to identify outlier oxides based on Bravais lattices that represented less than 2% of the total number of oxides. These outliers were removed from the dataset.

- **Heat Maps:** We used heat maps to validate the results of PCA and ensure that the data remained representative of the underlying distribution.

### Deep Neural Networks

For the prediction task, we employed deep neural networks. Here are the key steps in this phase:

- **Data Split:** We divided the dataset into three parts: 80% for training, 15% for validation, and the remaining 5% for testing.

- **Model Architecture:** We designed a feedforward deep neural network with four layers to capture complex relationships within the data.

- **Optimizer Comparison:** We compared the performance of two popular optimizers, ADAM and RMSProp, to fine-tune our model. Remarkably, both optimizers yielded an impressive R-squared (R2) score of 0.99.

- **Feature Impact Analysis:** We conducted an in-depth analysis to understand which features contributed most significantly to achieving the high R2 score. This knowledge can provide valuable insights into the factors influencing thermal conductivity in oxides.

### Extension to Nitrides and Sulphides

Building on our success with oxide materials, we extended our study to include nitrides and sulphides. While our model is particularly reliable for predicting the thermal conductivity of low-conductivity materials like oxides, this extension allows us to explore its applicability to other material types.

## Conclusion

This repository serves as a comprehensive resource for understanding and reproducing our work on predicting the thermal conductivity of oxides, nitrides, and sulphides using machine learning techniques. We hope our findings are valuable to the materials science community, and we encourage further exploration and research in this exciting field. If you have any questions or suggestions, please feel free to reach out.

---

*Please refer to the PDF presentation for a detailed overview of the project.*
