# Personalized Cancer_Diagnosis

![image](https://user-images.githubusercontent.com/61958476/117837430-13631b00-b297-11eb-86c8-124fe2e4a490.png)

## 1. Task: Classify the given genetic variations/mutations based on evidence from text-based clinical literature

### 1.1 In detail explaination:
1. Lets take a example where a person seems to have a symptoms of cancer and he visits a hospital where they basicaly remove the Cancer Tumor from person & then sequence those cancer tumor (genetic sequencing)
2. So after doing genetic sequencing of cancer tumor we get gene, gene mutation/variations where a small variation in a gene can cause cancer by destroying entire genetic core system 
3. Note: All types of Mutation does not cause cancer only few of them cause
4. So this is what we are going to do with help of features (gene , gene mutation ) we will predict 9 diffrent class labels and determine that out of which actually cause Cancer.

### 1.2. Workflow :
 1. Lets take a domain expert who understand about gene mutation, selects list of [genetic varaiations] he want to analyize.
    Genetic variations divide into 2 parts (1: gene {on which variation is happening} 2: varaiation {exact varations})
    Both can be considered as [Random Categorical Variables]
 2. Domain Expert will now search/ collect all research papers/ evidence/ text that has been done on this
    gene variations
 3. Spend some time on analyzing Text [i.e. Evidence / Reseach work] amd after that Determine that patient
    belongs to which of the class out of (1,2,3,4....,9)
    
#### Information gathered from: https://www.kaggle.com/c/msk-redefining-cancer-treatment/discussion/35336#198462

### 1.3 Data overview:
1. Training variants (ID,Gene,Variations,Classlabel)
2. Training_Texr (ID, TEXT)

### 1.4 Type of Machine learning problem
There are nine different classes a genetic mutation can be classified into => Multi class classification problem

### 1.5 Performance Metric
1. Multi-class Log loss
2. Confusion matrix

### 2. Exploratory Data Analysis 
#### 2.1 Distribution of Train,Test,Cv data  (64:20,16)

1. Train.csv
![image](https://user-images.githubusercontent.com/61958476/117840331-ae5cf480-b299-11eb-833f-9b9ddc7ec0ae.png)
Number of data points in class 1 : 609 ( 28.672 %)
Number of data points in class 2 : 439 ( 20.669 %)
Number of data points in class 3 : 363 ( 17.09 %)
Number of data points in class 4 : 289 ( 13.606 %)
Number of data points in class 5 : 176 ( 8.286 %)
Number of data points in class 6 : 155 ( 7.298 %)
Number of data points in class 7 : 57 ( 2.684 %)
Number of data points in class 8 : 24 ( 1.13 %)
Number of data points in class 9 : 12 ( 0.565 %)



