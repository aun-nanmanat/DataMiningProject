# Comparative Analysis of Imputation Techniques in Australian Rainfall Data
## Project Overview 
### Objective: 
Address the challenges of missing values in real-world datasets and evaluate the performance of various imputation techniques and machine learning models to improve the accuracy of predictive models for weather forecasting.

### Techniques Used: 
Data Imputation Techniques, with a focus on MICE (Multiple Imputation by Chained Equations), Machine Learning Model Evaluation including Random Forest Classifier (Scaled), Additional Techniques such as Cross-Validation, Learning Curve Examination, and Overfitting Analysis.

### Tools: 
Python (Pandas, Scikit-learn, MICE), R (tidyverse, caret).

### Key Findings:
- **Best Imputation Technique and Model:** MICE with Random Forest (Scaled) achieved top performance with 88.34% accuracy, 82.04% precision, and a ROC/AUC of 78.54%.

- **Cross-Validation:** Models with and without cross-validation showed similar stability and generalization capabilities.

- **Learning Curve Analysis:** Model performance improved significantly with more training data but showed diminishing returns beyond a certain point.

- **Overfitting:** Optimal model complexity was achieved with a maximum depth of 6 to 8 for Random Forest, balancing training and testing performance.

### Impact: Enhanced the reliability of rain prediction models by effectively handling missing values, contributing to more accurate weather forecasting.

## Executive Summary
Generally, it is undeniable that there are persistent challenges of missing values in real-world datasets, posing a significant threat to the integrity of analytical outcomes and the accuracy of predictive models. Therefore, our primary goal is to tackle these challenges of missing values in the datasets. This executive summary provides a comprehensive overview of our project “Comparative Analysis of Imputation Techniques in Australian Rainfall Data.” By employing systematic exploration, data preprocessing, imputation techniques, statistical methods, and machine learning models, our study seeks to advance our understanding of data preprocessing and missing value handling, explore the nuances of various imputation methodologies, and develop robust frameworks for assessing and interpreting the efficacy of different imputation strategies. Additionally, we expect to enhance the quality and reliability of weather predictions.

**Key Findings:**

***- Missingness Mechanism:*** A low p-value (typically < 0.05) suggests that our data is not randomly missing (MAR). This implies that the likelihood of missing values is influenced by other variables present in the dataset.

***- Top Performance of Imputation Technique and Model:*** The combination of MICE imputation method with the Random Forest (Scaled) model showed the highest performance, offering superior rain prediction in Australia with minimal computational overhead. Specifically, MICE achieved an accuracy of 88.34%, precision of 82.04%, and an ROC/AUC of 78.54%, marking it as the superior method for our specific dataset.

***- Cross-Validation Assessment:*** Both models with and without cross-validation exhibited similar accuracy and performance measures, indicating stability and effective generalization capability.

***- Learning Curve Examination:*** As the training data increases, the model achieves almost perfect scores, indicating its strong ability to remember the training set. However, beyond a certain point, adding more data leads to marginal performance improvements, suggesting diminishing returns.

***- Overfitting Analysis:*** Experimenting with various configurations of the Random Forest Classifier revealed fluctuations in performance metrics on the testing dataset, indicating potential overfitting. Optimal model complexity ranged from 6 to 8 for maximum depth, balancing training and testing performance. Estimator adjustments had limited impact beyond a certain threshold, emphasizing the trade-off between complexity and effectiveness.

## Conclusion
The comparative analysis of imputation techniques in Australian rainfall data reveals that careful consideration of imputation methods and model selection is crucial for accurate rain prediction. Our findings underscore the significance of addressing missing values effectively and highlight the potential of combining MICE imputation with the Random Forest (Scaled) model for superior performance. Moreover, our study emphasizes the importance of model stability, generalization ability, and the trade-off between complexity and effectiveness in machine learning tasks. Moving forward, further exploration of feature engineering methods, alternative algorithms, and ensemble techniques could enhance rain prediction accuracy in Australia, contributing to advancements in weather forecasting and decision-making processes.

## References

A. Picornell, J. Oteros, R. Ruiz-Mata, M. Recio, M.M. Trigo, M. Martínez-Bracero, B. Lara, A. Serrano-García, C. Galán, H. García-Mozo, P. Alcázar, R. Pérez-Badia, B. Cabezudo, J. Romero-Morte, J. Rojo. (2021). Methods for interpolating missing data in aerobiological databases. Environmental Research.[https://doi.org/10.1016/j.envres.2021.111391](https://doi.org/10.1016/j.envres.2021.111391)

Alhamid, M. (2020, December 24). What is Cross-Validation? Testing your machine learning models with cross-validation. Towards Data Science. [https://towardsdatascience.com/what-is-cross-validation-60c01f9d9e75](https://towardsdatascience.com/what-is-cross-validation-60c01f9d9e75)

Ali, Aida & Shamsuddin, Siti Mariyam & Ralescu, Anca. (2015). Classification with class imbalance problem: A review. 7. 176-204. UTM Big Data Centre, Ibnu Sina Institute for Scientific and Industrial Research Universiti Teknologi Malaysia.[https://www.researchgate.net/publication/288228469_Classification_with_class_imbalance_problem_A_review](https://www.researchgate.net/publication/288228469_Classification_with_class_imbalance_problem_A_review) 

Aliferis, C., Simon, G. (2024). Overfitting, Underfitting, and General Model Overconfidence and Under-Performance Pitfalls and Best Practices in Machine Learning and AI. Artificial Intelligence and Machine Learning in Health Care and Medical Sciences. Health Informatics. Springer, Cham. [https://doi.org/10.1007/978-3-031-39355-6_10](https://doi.org/10.1007/978-3-031-39355-6_10)

Alves, L. M. (2021, July 2). KNN (K Nearest Neighbors) and KNeighborsClassifier — What it is, how it works, and a practical…[https://luis-miguel-code.medium.com/knn-k-nearest-neighbors-and-kneighborsclassifier-what-it-is-how-it-works-and-a-practical-914ec089e467](https://luis-miguel-code.medium.com/knn-k-nearest-neighbors-and-kneighborsclassifier-what-it-is-how-it-works-and-a-practical-914ec089e467)

Azur, M. J., Stuart, E. A., Frangakis, C., & Leaf, P. J. (2011). Multiple imputation by chained equations: what is it and how does it work? International journal of methods in psychiatric research, 20(1), 40–49. [https://doi.org/10.1002/mpr.329](https://doi.org/10.1002/mpr.329)

Blagec, K., Dorffner, G., Moradi, M., & Samwald, M. (2020). A critical analysis of metrics used for measuring progress in artificial intelligence. Section for Artificial Intelligence and Decision Support; Center for Medical Statistics, Informatics, and Intelligent Systems; Medical University of Vienna. [https://arxiv.org/pdf/2008.02577](https://arxiv.org/pdf/2008.02577)

Gabr, M., Ibrahim, Y., Mostafa H., & Doaa S. E. (2023). Effect of Missing Data Types and Imputation Methods on Supervised Classifiers: An Evaluation Study. Big Data and Cognitive Computing 7, no. 1: 55. [https://doi.org/10.3390/bdcc7010055](https://doi.org/10.3390/bdcc7010055)

Giola, C., Danti, P., & Magnani, S. (2021, July 13). Learning curves: A novel approach for robustness improvement of load forecasting. *MDPI.* [https://www.mdpi.com/2673-4591/5/1/38#metrics](https://www.mdpi.com/2673-4591/5/1/38#metrics)

Hameed, W. & Ali, N. (2023). Missing value imputation Techniques: A Survey. UHD Journal of Science and Technology. [https://www.researchgate.net/publication/369674417_Missing_value_imputation_Techniques_A_Survey](https://www.researchgate.net/publication/369674417_Missing_value_imputation_Techniques_A_Survey)

IBM. (2022). What Is Logistic Regression? IBM.[https://www.ibm.com/topics/logistic-regression](https://www.ibm.com/topics/logistic-regression)

IBM. (2023a). What is a Decision Tree | IBM.[https://www.ibm.com/topics/decision-trees](https://www.ibm.com/topics/decision-trees)

IBM. (2023b). What is Random Forest? | IBM.[https://www.ibm.com/topics/random-forest](https://www.ibm.com/topics/random-forest)

Jason B. (2018, November 20). A Gentle Introduction to the Gradient Boosting Algorithm for Machine Learning. Machine Learning Mastery.[https://machinelearningmastery.com/gentle-introduction-gradient-boosting-algorithm-machine-learning/](https://machinelearningmastery.com/gentle-introduction-gradient-boosting-algorithm-machine-learning/)

Jiaxu P., Jungpil H., Ke-Wei H. (2022) Handling Missing Values in Information Systems Research: A Review of Methods and Assumptions. Information Systems Research 34(1):5-26. [https://doi.org/10.1287/isre.2022.1104](https://doi.org/10.1287/isre.2022.1104)

Kang H. (2013). The prevention and handling of the missing data. Korean Journal of Anesthesiology, 64(5), 402–406. [https://doi.org/10.4097/kjae.2013.64.5.402](https://doi.org/10.4097/kjae.2013.64.5.402)

Kavya, D. (2023, February 15). Optimizing Performance: SelectKBest for Efficient Feature Selection in Machine Learning. Medium. [https://medium.com/@Kavya2099/optimizing-performance-selectkbest-for-efficient-feature-selection-in-machine-learning-3b635905ed48](https://medium.com/@Kavya2099/optimizing-performance-selectkbest-for-efficient-feature-selection-in-machine-learning-3b635905ed48)

Makaba, T. & Dogo, E. (2019). A Comparison of Strategies for Missing Values in Data on Machine Learning Classification Algorithms. International Multidisciplinary Information Technology and Engineering Conference (IMITEC), Vanderbijlpark, South Africa, pp. 1-7. [https://ieeexplore.ieee.org/document/9015889](https://ieeexplore.ieee.org/document/9015889)

Ribeiro, D. (2023). Missing values in data analysis: A comprehensive guide. Medium. [https://medium.com/data-science-as-a-better-idea/missing-values-in-data-analysis-a-comprehensive-guide-2151bc2e8579](https://medium.com/data-science-as-a-better-idea/missing-values-in-data-analysis-a-comprehensive-guide-2151bc2e8579)

Padgett, C. & Skilbeck, C. & Summers, M. (2014). Missing Data: The 
Importance and Impact of Missing Data from Clinical Research. Brain Impairment. [https://www.researchgate.net/publication/262036960_Missing_Data_The_Importance_and_Impact_of_Missing_Data_from_Clinical_Research](https://www.researchgate.net/publication/262036960_Missing_Data_The_Importance_and_Impact_of_Missing_Data_from_Clinical_Research)

Salgado, C.M., Azevedo, C., Proença, H., & Vieira, S.M. (2016). Missing Data. In: Secondary Analysis of Electronic Health Records. Springer, Cham. [https://doi.org/10.1007/978-3-319-43742-2_13](https://doi.org/10.1007/978-3-319-43742-2_13)

Song, Q. & Shepperd, M. (2007). Missing Data Imputation Techniques. 
International Journal of Business Intelligence and Data Mining. [https://www.researchgate.net/publication/220579612_Missing_Data_Imputation_Techniques](https://www.researchgate.net/publication/220579612_Missing_Data_Imputation_Techniques)

Torres, M. & Juan, A. (2014). Comparison of imputation methods for handling missing categorical data with univariate patterns. Revista de Métodos Cuantitativos para la Economía y la Empresa, ISSN 1886-516X, Universidad Pablo de Olavide, Sevilla, Vol.17, pp. 101-120. [https://hdl.handle.net/10419/113873](https://hdl.handle.net/10419/113873)

Wizards, D. S. (2023, July 7). Understanding the AdaBoost Algorithm. Medium.[https://medium.com/@datasciencewizards/understanding-the-adaboost-algorithm-2e9344d83d9b](https://medium.com/@datasciencewizards/understanding-the-adaboost-algorithm-2e9344d83d9b)
