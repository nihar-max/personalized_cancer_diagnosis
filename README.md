# Personalized Cancer_Diagnosis

![image](https://user-images.githubusercontent.com/61958476/117837430-13631b00-b297-11eb-86c8-124fe2e4a490.png)

## 1. Task: Classify the given genetic variations/mutations based on evidence from text-based clinical literature

### 1.1 In detail explaination:
1. Lets take a example where a person seems to have a symptoms of cancer and he visits a hospital where they basicaly remove the Cancer Tumor from person & then sequence those cancer tumor (genetic sequencing)
2. So after doing genetic sequencing of cancer tumor we get gene, gene mutation/variations where a small variation in a gene can cause cancer by destroying entire genetic core system 
3. Note: All types of Mutation does not cause cancer only few of them cause
4. So this is what we are going to do with help of features (gene , gene mutation ) we will predict 9 diffrent class labels and determine that out of which actually cause Cancer.

### 1.2. Workflow :
 1 : Lets take a domain expert who understand about gene mutation, selects list of [genetic varaiations] he want to analyize.
    Genetic variations divide into 2 parts (1: gene {on which variation is happening} 2: varaiation {exact varations})
    Both can be considered as [Random Categorical Variables]
 2 : Domain Expert will now search/ collect all research papers/ evidence/ text that has been done on this
    gene variations
 3 : Spend some time on analyzing Text [i.e. Evidence / Reseach work] amd after that Determine that patient
    belongs to which of the class out of (1,2,3,4....,9)
