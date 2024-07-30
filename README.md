# classification-of-mice-based-on-protein-expression-levels

This project was introduced by Evoastra Ventures Pvt. Ltd. 
This project was about Classification of Mice Based on Protein Expression Levels.
Problem Statement
The goal of this project is to analyze protein expression levels in the cerebral cortex of mice to classify them into different categories based on their genotype, behavior, and treatment. Specifically, the project aims to identify subsets of proteins that can discriminate between these classes and to understand the biological mechanisms underlying learning and memory, particularly in the context of Down syndrome.


Objective
Classify Mice Based on Protein Expression: Develop a machine learning model to accurately classify mice into one of the eight classes based on the expression levels of 77 proteins. These classes are determined by a combination of genotype (control or trisomic), behavior (stimulated to learn or not), and treatment (saline or memantine).
Identify Key Discriminant Proteins: Utilize feature selection techniques to identify which proteins or protein modifications are most important for distinguishing between the different classes. Understanding which proteins are key discriminators can provide insights into the biological mechanisms underlying learning and memory in Down syndrome.
Evaluate the Impact of Genotype, Behavior, and Treatment: Analyze the effect of genotype (control vs. trisomic), behavior (context-shock vs. shock-context), and treatment (saline vs. memantine) on protein expression levels. This includes evaluating how these factors influence associative learning and the potential therapeutic effects of memantine in trisomic mice.


Dataset Description
The dataset consists of the expression levels of 77 proteins/protein modifications measured in the nuclear fraction of the cerebral cortex in mice. The data is collected from both control mice and trisomic (Down syndrome) mice, subjected to a context fear conditioning task to assess associative learning.


Dataset Characteristics:
Type: Multivariate
Subject Area: Biology
Associated Tasks: Classification, Clustering
Feature Type: Real
Instances: 1080
Features: 80

Breakdown:
Mice Classes: 8 (based on genotype, behavior, and treatment)
Control Mice:
c-CS-s: Control, Stimulated, Saline (9 mice)
c-CS-m: Control, Stimulated, Memantine (10 mice)
c-SC-s: Control, Not Stimulated, Saline (9 mice)
c-SC-m: Control, Not Stimulated, Memantine (10 mice)
Trisomic Mice:
t-CS-s: Trisomic, Stimulated, Saline (7 mice)
t-CS-m: Trisomic, Stimulated, Memantine (9 mice)
t-SC-s: Trisomic, Not Stimulated, Saline (9 mice)
t-SC-m: Trisomic, Not Stimulated, Memantine (9 mice)

Details:
Control Mice: 38 mice, 570 measurements (15 measurements per protein per mouse)
Trisomic Mice: 34 mice, 510 measurements (15 measurements per protein per mouse)
Total Measurements: 1080 measurements per protein

Features:
Protein Expression Levels: 77 proteins/protein modifications.
Additional Features: Mouse ID, Genotype, Treatment.

I had worked in a team during this project. My part in the project was to perform feature selection and model training. I had utilized Random Forest Classifier Feature Importance and SelectKBest with F-test for selecting the best predictors. After performing these steps we used median to find out the threshold point for the predictors. Only the predictors with value more than threshold points were to be selected. After finding the predictors from each Feature Importance Technique performed, then used the common predictors that were found. Then I had worked with various Machine Learning models such as Random Forest Classifier, Decision Tree Classifier and XGBoost Classifier. Only Random Forest Classifier and XGBoost Classifier were included in the final code. I had also performed hypertuning to find out about the best params using which we can optimize the Machine Learning models for optimized results.
