# Stellar Object Classification - Project README 
## Problem Statement
The field of astronomy relies heavily on accurate and efficient classification of celestial objects. The Sloan Digital Sky Survey (SDSS) provides a rich dataset with columns such as 'u', 'g', 'r', 'i', 'z', 'class', and 'redshift'. The challenge is to develop a robust classification model that accurately identifies the class of celestial objects based on their spectral features. The goal of this project is to create a model that accurately distinguishes between types of stellar objects from Sloan Digital Sky Survey (SDSS) data to help physicists more finely distinguish quasars, galaxies, and stars.



| Feature    | Type    | Dataset | Description                                        |
|------------|---------|---------|----------------------------------------------------|
| u          | float   | SDSS    | Ultraviolet filter in the photometric system              |
| g          | float   | SDSS    |  Green filter in the photometric system              |
| r          | float   | SDSS    | Red filter in the photometric system              |
| i          | float   | SDSS    | Near Infrared filter in the photometric system        |
| z          | float   | SDSS    | Infrared filter in the photometric system        |
| class      | string  | SDSS    | Class of celestial object (e.g., star, galaxy, quasar) |
| redshift   | float   | SDSS    | Redshift value usually indicating the object's distance from Earth.  Redshift is a constant multiple to all wavelengths of the spectrum emmitted by stellar objects|

# Executive Summary
## Problem Overview
The classification of celestial objects is a fundamental task in astronomy, and the SDSS dataset, comprising 500,000 data points, provides an opportunity to enhance the accuracy and efficiency of this process. The project aims to leverage machine learning techniques to develop a classification model for celestial objects based on their spectral features.

## Goals and Objectives
* Develop a machine learning model for classifying celestial objects.
* Achieve a classification accuracy of at least 98% on the test dataset.
## Methodology
The project involves the following steps:

1. Data exploration and understanding of the SDSS dataset obtained through a SQL query.
2. Data preprocessing, including handling missing values and encoding categorical variables.
3. Model selection and training using appropriate machine learning algorithms.
4. Evaluation of the model on a held-out test dataset.
## Key Findings
* The developed model achieves a classification accuracy of 99.4% on the test dataset.
* Notably, there is a significant difference in redshift for quasars misclassified by the random forest model.
## Redshift Anomaly
During the analysis, it was observed that the random forest model misclassified certain quasars, and further investigation revealed a notable difference in redshift values for these instances. This finding may provide evidence supporting the anomaly in lower than expected redshifts for certain quasars, a phenomenon that cannot be currently explained by existing astronomical models.

## Conclusion
The project successfully addresses the challenge of celestial object classification using the SDSS dataset obtained through a SQL query. The developed model demonstrates high accuracy, and the observed redshift anomaly in misclassified quasars adds an intriguing layer to the research.

##Next Steps
1. Explore additional feature engineering techniques to enhance model performance.
2. Investigate the underlying causes of the redshift anomaly in misclassified quasars.
3. Collaborate with astronomers and domain experts to gather insights for further refinement.
4. Consider expanding the project to include a broader range of celestial objects or additional datasets.

By taking these next steps, the project can continue to evolve and provide even more accurate and meaningful results in the field of astronomy, potentially contributing to our understanding of celestial phenomena.