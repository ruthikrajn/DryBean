# Dry Bean Classification
## Final Project – Planning & Description


**Author**:  
- Ruthik Raj Nataraja  

**Under the Guidance of Professors**:  
- Siddhartha Putti  
- Ramin Mohammadi  
- Sachini Weerasekara  

---

## About the Dataset

The dataset contains information on **seven different types of dry beans**. It includes **17 attributes** and a total of **13,611 instances**. These features are numerical (both integer and real-valued) and suitable for classification tasks. The beans are classified into the following types:

- **Seker**  
- **Barbunya**  
- **Bombay**  
- **Cali**  
- **Dermosan**  
- **Horoz**  
- **Sira**

The features include:  
`Area`, `Perimeter`, `Major Axis Length`, `Minor Axis Length`, `Aspect Ratio`, `Eccentricity`, `Convex Area`, `Equivalent Diameter`, `Extent`, `Solidity`, `Roundness`, `Compactness`, and `Shape`.

These attributes were extracted using **computer vision** techniques after bean images were processed through **segmentation** and **feature extraction** stages.

**Data Source**:  
UCI Machine Learning Repository  
[Dry Bean Dataset](https://archive.ics.uci.edu/ml/datasets/dry+bean+dataset)

---

## Goal of the Project

The primary goal is to build a **machine learning model** that can accurately classify dry bean types based on the extracted features.

Manual classification of dry beans is **time-consuming and costly**, especially at scale. Automating this process using machine learning can:

- **Improve classification accuracy**
- **Reduce manual labor**
- **Enhance processing speed in agricultural and food processing industries**

---

## Approach

To achieve uniform seed classification, we will follow a systematic approach, starting with data preparation and feature selection/extraction techniques like **PCA** and **SMOTE**. By using these methods, we can enhance the quality and performance of our multiclass classification models.

Our dataset contains features collected by a computer vision system, enabling us to classify beans accurately into their respective categories.

### Models to be Used:

1. **Linear Discriminant Analysis (LDA)**  
   LDA is suitable for multiclass problems. Before applying LDA, we will verify if the data meets the assumptions of LDA and make necessary modifications to the data accordingly.

2. **Logistic Regression**  
   Logistic regression is a versatile model that can be used for multiclass classification. By calculating probabilities for each class using the SoftMax function, we can classify instances accordingly. Logistic regression performs well when the data is linearly separable.

3. **Naïve Bayes**  
   We will assess the conditional independence assumption between features before applying the Gaussian Naïve Bayes algorithm for classification. Naïve Bayes models can be effective when features are conditionally independent.

4. **Neural Network**  
   We will develop a Neural Network model with multiple layers and nodes to classify the classes. Neural networks excel at capturing complex patterns in the data, making them suitable for the task at hand.

---

## Hyperparameter Tuning

After developing all the models, we will tune hyperparameters to improve performance. The best-performing model will be chosen based on the comparison of performance scores across all models.

---

## Conclusion

This project aims to develop a robust machine learning model to automate the classification of dry beans, saving time and resources in the agricultural and food processing industries. By leveraging advanced machine learning techniques, we can significantly improve the accuracy and efficiency of bean classification, ensuring better quality control and optimized pricing based on bean quality.

