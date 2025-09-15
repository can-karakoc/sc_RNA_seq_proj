# scRNA Sequence Analysis and Classification Project
**Personal Project** by Can Karakoc  
**Duration:** August - September 2025  
**Dataset:** [3k PBMCs Data from Healthy Donor by 10X Genomics](https://www.10xgenomics.com/datasets/3-k-pbm-cs-from-a-healthy-donor-1-standard-1-1-0)  
**Tools:** Python, ScanPy, scikit-learn, PyTorch, Pandas, Matplotlib, Seaborn  
**License:** Open-source

This project analyzes single-cell RNA sequencing (scRNA-seq) data from 3,000 peripheral blood mononuclear cells (PBMCs) of a healthy donor, provided by 10X Genomics. The main goals of the project were to explore different data processing, classification techniques, and visualization methods learned in coursework, using open-source data for a classification problem.  

- **Data preprocessing and clustering:** Cleaning and organizing scRNA-seq data to uncover cellular heterogeneity.  
- **Exploratory analyses and visualizations:** Applying various visualization techniques to better understand the dataset.  
- **Classification comparison:** Implementing multiple classification algorithms and comparing their performance using confusion matrices.  
- **Results summary:** Model accuracies are presented in the table below for easy comparison.  

This workflow demonstrates an end-to-end approach to single-cell data analysis while applying practical machine learning techniques. The accuricies of the models explored in the project are presented below:


|Model                                  |Accuracy          |Macro-F1          |
|---------------------------------------|------------------|------------------|
|Logistic Regression                   |0.9545454545454546|0.9637717239786943|
|Random Forest                          |0.9526515151515151|0.9621167098554327|
|CellClassify Neural Net                |0.9545454545454546|0.9644901735147453|
|Random Forest on Autoencoder Embeddings|0.9299242424242424|0.9412082669966715|

[Go to Results.csv](results/model_benchmark.csv)

 ## Discussion and Results

This project demonstrates how immune cell heterogeneity can be studied by scRNA-seq preprocessing and supervised classification. Through quality control, normalization, and feature selection, biologically meaningful cell clusters were obtained from raw sequencing data. Annotation with canonical marker genes confirmed the expected immune subtypes in PBMCs.

The classification step compared traditional machine learning models (logistic regression, random forest, and neural networks). Despite differences in complexity, all models achieved strong performance, indicating that the preprocessing pipeline effectively distilled informative features. The neural network provided slightly better flexibility, while logistic regression offered interpretability.

Overall, this project highlights both the strengths and trade-offs of classical and deep learning approaches in single-cell analysis. It also illustrates how open-source biomedical data can be leveraged to explore diverse preprocessing, classification, and visualization techniques.
