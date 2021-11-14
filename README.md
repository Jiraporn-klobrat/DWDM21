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
  * [Data Preprocessing](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Data_Preprocessing_(Chapter_3).ipynb)
    * Meta Data (Data ที่ใช้อธิบาย Data)
      * ชี้ข้อมูลในตาราง
        * ชี้แบบธรรมดา ใช้ [ชื่อ column][index]
        * ชี้แบบ .iloc[] (มองข้อมูลเป็น matrix)
      * Missing Values
        * Handling Missing Value 1 (ลบค่า missing)
        * Quiz 3 ให้หาว่า การทำ dropna() ทำให้ข้อมูลหายไปกี่ %
        * Handling Missing Value 1.5 (ลบค่า missing เฉพาะใน คอลัมล์ที่เราสนใจเท่านั้น)
        * Quiz 3.1 ให้ หาว่า การทำ dropna() แบบเลือก drop เฉพาะ คอลัมล์ที่เราสนใจ ทำให้ข้อมูลหายไป กี่%
        * แก้ไขควิซ
        * Handling Missing Value 2 (แทนด้วย class ใหม่ (unknown))
        * Handling Missing Value 3 (แทนด้วย class ใหม่ (ค่าที่เหมาะสม))
        * Handling Missing Value 4 (แทนด้วย ค่ากลาง)
          * ถ้าเป็น numeric ใช้ mean
          * ถ้าเป็น norminal (ตัวหนังสือ) จะใช้ mode
          * ถ้าเป็น ordinal ใช้ median
            * เติมด้วยค่าของ column ใกล้เคียง (เดี๋ยวย้อนกลับมา)
        * Handling Missing Value 5 (แทนด้วย ค่ากลางของ samples ใน class เดียวกัน)
      * Select data by values [PD]
        * สร้าง list ของ boolean
          * นำ list ของ boolean มาเลือกค่าในตาราง
      * Quiz 4 + HW
          * records ที่ กักตัวที่ขอนแก่น
          * records ที่ กักตัวที่ ขอนแก่น+โคราช+อุดร
          * records ที่ เป็นผู้หญิงที่พบเชื้อที่ กทม
          * records ที่เป็นผู้ชาย อายุ 18-22 ปี ที่กักตัวที่เชียงใหม่
          * หาอายุเฉลี่ยของคนที่พบเชื้อที่ ขอนแก่น
            * พบที่ขอนแก่น
            * เอาค่า mean ไปเติมตรง missing column 'age'
            * ต่อตารางแนวแกน Y [PD]
        * Handling Missing Value 5 (แทนด้วย ค่ากลางของ samples ใน class เดียวกัน)(ต่อ)
        * การเรียงข้อมูล [PD]
      * Outlier
        * ตัด outlier แบบ manual
      * Quiz 5
      * HW หรือ Quiz กลุ่ม (III) แก้ให้ function box_vals สามารถรับ input ที่ box plot วาดแบบแนวนอนได้ (vert = False)
      * Pandas' looping (.iterrows)
      * การรวมตาราง Data Integration (ต่อตารางในแนวแกน x)
        * รวม 2 ตาราง (.merge())
        * เลือกเฉพาะ column ที่ต้องการมาแปะ (.map())
        * ตารางรอง (ตารางข้างขวา) ต้องไม่มี index ซ้ำ
        * Group by (pandas)
        * HW + Quiz
          * (จากตาราง w_restaurant กับ search_click) หา จังหวัดที่มีคนกดเข้าไปดูผลการ search 3 อันดับแรก
          * (จากตาราง w_restaurant กับ search_click) เมืองไหนที่มีค่าเฉลี่ยของ 'weighted_average_rating' สูงที่สุด
          * (จากตาราง confirmed-cases) เรียงลำดับ risk ที่ทีให้คนติดโรค 5 อันดับแรก
          * (จากตาราง confirmed-cases) หาจังหวัดที่มีคนกักตัวมากที่สุด 10 อันดับแรก
          * เฉลย HW10 + Quiz
         * [PD] save ตารางเอาไปใช้ที่อื่น
         * [PD] การสร้างตาราง


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
  * [Data 'reduced_marketbasket' Case](https://github.com/Jiraporn-klobrat/DWDM21/blob/main/Chapter6_Association_Rules.ipynb)
    * ลบ records ที่ถูก cancel ออกไป
    * [Q] มีประเทศสาขาของ supermarket นี้ทั้งหมดกี่ประเทศ
    * [HW13] วาดกราฟสรุปจำนวน items และ ยอดขายของแต่ละประเทศ
    * เฉลยการบ้าน
      * ดูว่า คอลัมน์ไหนมี ค่า missing บ้าง
      * เพิ่มคอลัมน์ ยอดขาย (Quantity*UnitPrice)
      * เตรียม Data สำหรับ (Fequence Pattern) Association Rule
    * Apriori
      * (Quiz7) หา k-itemset ที่มีความน่าสนใจ (โดยพิจารณาลูกค้าเป็นรายคน) พร้อมทั้งอธิบายว่าน่าสนใจยังไง
      * แก้ไข Quiz7



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
