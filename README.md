# DWDM21
## Data Warehouse &amp; Data Mining 2021

นางสาวจิราพร กลบรัตน์ 623020762-6

ชื่อกลุ่ม: เอกาไร้สติ

1 **นางสาวจิราพร กลบรัตน์ 623020762-6**

2 นางสาวกัญญาวีร์ ศรีเทียมเงิน 623020511-1

3 นางสาวชลธิชา ศาลางาม 623020518-7

4 นางสาวสุภาภรณ์ บุตุธรรม 623020543-8

5 นางสาววิกานดา หงษ์บุญมี 623020764-2


# สารบัญ
* บทที่ 1 INTRODUCTION 
   * [Lecture Introduction](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chapter%201.pdf)
      * Data Mining?
      * Knowledge Discovery (KDD) Process
      * Example: A Web Mining Framework
      * Data Mining in Business Intelligence
      * How the data suppose to look like
      * Data Mining Functions
        * Pattern Discovery
        * Classification
        * Cluster Analysis

* บทที่ 2 Getting to Know Your Data
  * [Lecture Data Objects and Attribute Types](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chapter%202.pdf)
    * Types of Data Sets
      * Record Data
      * Ordered Data
      * Spatial, image and multimedia Data
    * Important Characteristics of Structured Data
    * Data Objects
    * Attributes
    * Attribute Types
    * Numeric Attribute Types
    * Discrete Attribute
    * Continuous Attribute
    * Basic Statistical Descriptions of Data

  * [Lecture Measuring Data Similarity and Dissimilarity](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chapter%202%20%E0%B9%80%E0%B8%9E%E0%B8%B4%E0%B9%88%E0%B8%A1%E0%B9%80%E0%B8%95%E0%B8%B4%E0%B8%A1.pdf)
    * Similarity, Dissimilarity, and Proximity
    * Data Matrix and Dissimilarity Matrix
    * Standardizing Numeric Data
    * Special Cases of Minkowski Distance

  * [Lecture Binary Distance](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chapter%202%20Binary%20Distance_140964.pdf)
    * Proximity Measure for Binary Attributes
    * Proximity Measure for Categorical Attributes
    * Ordinal Variables
    * Attributes of Mixed Type
    * Cosine Similarity of Two Vectors


* บทที่ 3 Data Preprocessing
  * [Lecture Data Preprocessing](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chapter%203.pdf)
    * Data Preprocessing: An Overview
    * Data Cleaning


* บทที่ 4 Data Warehousing and On-line Analytical Processing
  * [Lecture Data Warehousing and On-line Analytical Processing](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chapter%204.pdf)
    * What is a Data Warehouse?
    * From Tables and Spreadsheets to Data Cubes
    * Conceptual Modeling of Data Warehouses
       * Star Schema: An Example
       * Snowflake Schema: An Example
       * Fact Constellation: An Example
     * Typical OLAP Operations
        * Roll up (drill-up)
        * Drill down (roll down)
        * Slice and dice
        * Pivot (rotate)
        * Drill across
        * Drill through


* บทที่ 5 Association Rules
  * [Lecture Mining Frequent Patterns, Association and Correlations: Basic Concepts and Methods](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chapter%206.pdf)
    * Basic Concepts
      * What Is Pattern Discovery?
        * k-Itemsets and Their Supports
        * Frequent Itemsets (Patterns)
        * From Frequent Itemsets to Association Rules
        * Mining Frequent Itemsets and Association Rules
    * Efficient Pattern Mining Methods
      * Apriori Algorithm
        * Apriori Pruning and Scalable Mining Methods
        * A Candidate Generation & Test Approach
        * The Apriori Algorithm


* บทที่ 6 Classification
  * [Lecture Classification: Basic Concepts](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chapter%208.pdf)
    * Basic Concepts
      * Supervised vs. Unsupervised Learning (1)
      * Supervised vs. Unsupervised Learning (2)
      * Prediction Problems: Classification vs. Numeric Prediction
      * Classification—Model Construction, Validation and Testing
    * Decision Tree Induction
      * An Example
      * Information Gain
  * [HW Decision Tree คำนวณมือ](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Decision%20Tree_%E0%B8%84%E0%B8%B3%E0%B8%99%E0%B8%A7%E0%B8%93%E0%B8%A1%E0%B8%B7%E0%B8%AD.pdf)
  * [Lecture Decision Tree](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chapter%208%20Lecture%20%E0%B9%80%E0%B8%9E%E0%B8%B4%E0%B9%88%E0%B8%A1%E0%B9%80%E0%B8%95%E0%B8%B4%E0%B8%A1.pdf)
  * [Decision Tree](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chapter7_Classification(Decision_Tree).ipynb)
    * Load Data
    * Train Model
      * import (เรียกใช้ algorithm ที่เราต้องการ)
      * define (กำหนด parameters ให้กับ model)
      * train (ฝึกสอนตัวแบบ)
    * Plot tree
    * Evalution
      * Random
    * Advanced Tree
      * Import
      * Define
      * Train
    * TEST
    * Start here
      * Import
      * Define
      * Train
      * Evaluate
    * HW
      * ต้นไม้ที่ใช้เกณฑ์ Entropy มีความสูงไม่เกิน 4 ชั้น
        * Import
        * Define
        * Train
        * Evaluate
      * ต้นไม้ที่ใช้เกณฑ์ Gini มีใบไม่เกิน 25 ใบ
        * import
        * Define
        * Train
        * Evaluate
      * ต้นไม้ที่ใช้เกณฑ์ Entropy และใช้การ split แบบ random
        * import
        * Define
        * Train
        * Evaluate
      * ต้นไม้ที่เราคิดเอง
        * import
        * Define
        * Train
        * Evaluate
      * เลือก mytreeNo3 แล้ว train ใหม่ด้วย Training
  * [Lecture k-Nearest Neighbor](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Lecture%20%E0%B9%80%E0%B8%9E%E0%B8%B4%E0%B9%88%E0%B8%A1%E0%B9%80%E0%B8%95%E0%B8%B4%E0%B8%A1.pdf)
    * Bayes’ Theorem: Basics
    * Naïve Bayes Classifier
      * Categorical vs. Continuous Valued Features
      * Training Dataset
    * Lazy Learner: Instance-Based Methods
    * The k-Nearest Neighbor Algorithm
  * [Lecture Evaluation & Neural Networks](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Precision_Recall_F-measures.pdf)
    * Neural Network for Classification
      * Perceptron
    * Model Evaluation and Selection
    * Classifier Evaluation Metrics
      * Confusion Matrix
      * Accuracy, Error Rate,Sensitivity and Specificity
      * Precision and Recall, and F-measures
  * [k-Nearest Neighbor & Neural Networks](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chap7_Classification(KNN_NN).ipynb)
    * Load Data
    * Split Data
    * Train Model
      * import
      * knn1
      * knn2
      * knn3
    * Retrain & Evaluate
    * Neural Network
      * Import
      * Define
      * Train - Test
      * ANN 2
      * ANN 3  
  * [Evaluation](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chap7_Classification_(Evaluation).ipynb)
    * Load data
    * แบ่ง Data
    * สร้าง Model ทำนาย
      * Import
      * Define
      * Train
    * Evaluation


* บทที่ 7 Clustering
  * [Clustering](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chap8_Clustering.ipynb)
    * K-means
      * Generate Data
      * Explore Data
      * Clustering
        * Import
        * Define
        * Fit-Predict
        * Plot
      * Example Application (Color Quantization)
        * นับจำนวนสี
        * จัดกลุ่มสีให้เหลือ 16 สี
        * ใช้ centroid เป็นตัวแทนของสี


* MiniExam
  * [MiniExam](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/MiniExam.ipynb)


* Group Project
