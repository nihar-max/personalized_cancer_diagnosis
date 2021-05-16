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
#### Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/data
1. Training variants (ID,Gene,Variations,Classlabel)
2. Training_Texr (ID, TEXT)

### 1.4 Type of Machine learning problem
There are nine different classes a genetic mutation can be classified into => Multi class classification problem

### 1.5 Performance Metric
1. Multi-class Log loss
2. Confusion matrix

### 2. Exploratory Data Analysis 
#### 2.1 Distribution of Train,Test,Cv data  (64:20,16)

##### Distribution of yi in Train

![image](https://user-images.githubusercontent.com/61958476/117840331-ae5cf480-b299-11eb-833f-9b9ddc7ec0ae.png)

##### Distribution of yi in Test

![image](https://user-images.githubusercontent.com/61958476/117840724-0d226e00-b29a-11eb-9d67-056760d5e116.png)

##### Distribution of yi in CV
![image](https://user-images.githubusercontent.com/61958476/117840804-1c092080-b29a-11eb-95c6-113d7b64aa1e.png)

#### Observation: Here we have done Stratified Train Test CV split so that we get equal amount of distribution in all 3 plots as we can see and by looking at this Histogram we can come into concluison that Class Label {7,4,1,2} consist of more than 60% - 70% of data and so this is an Imbalanced Dataset 

### 2.1 Univariate Analysis
#### 2.1.2 Univariate Analysis on Gene feature

##### Q.How many categories are there and How they are distributed?
    unique_genes = train_df["Gene"].value_counts()
>>>> (240,)

##### Plot CDF for this distrbutions of gene feature
    s = sum(unique_genes.values)
    h = unique_genes.values/s
    c = np.cumsum(h)
    plt.plot(c,label='Cumulative distribution of Genes')
    plt.grid()
    plt.legend()
    plt.show()
    
![image](https://user-images.githubusercontent.com/61958476/118019833-0f0e2f00-b377-11eb-91f2-9831870be97b.png)

Observation: Out of 225 unique genes only top 50 genes consist more than 70% of data and rest only 30%

#### 2.1.3 Univariate Analysis on Variation feature

##### Q.How many categories are there and How they are distributed?
    unique_genes = train_df["Variation"].value_counts()
>>> (1941,)

##### Plot CDF for this distrbutions of gene feature
    s = sum(unique_variation.values)
    h = unique_variation.values/s
    c = np.cumsum(h)
    plt.plot(c,label='Cumulative distribution of Genes')
    plt.grid()
    plt.legend()
    plt.show()
    
![image](https://user-images.githubusercontent.com/61958476/118392874-7539d100-b659-11eb-8218-93ba92c78950.png)

## 3. Machine Learning models used
### 1. Multinomial Naive Bayes 
### 1. Multinomial Naive Bayes 
### 1. Multinomial Naive Bayes 
### 1. Multinomial Naive Bayes 
### 1. Multinomial Naive Bayes 






