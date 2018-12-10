# Precision Medicine - Where do we go from here?
### by Mengyi Liu (Miko)

### Sections:
##### 1. Introduction to Precision Medicine
##### 2. Personalized Medicine through the Lens of Asthma
##### 3. Current Hot Topics on Precision Medicine

## 1. Introduction to Precision Medicine
Definition of Precision Medicine: Tailoring of medical treatment to the individual characteristics of each patient, especially by using genetic or molecular profiling.

To advance the field, current genomics and machine learning researchers need to address:

- identifying genetic or molecular markers for clinical phenotypes
- discovering disease subtypes from genetic and/or molecular data
- building prediction models for clinical events based on electronic medical record (EMR) data

> Let's look at an example where scientists used the theory of precision medicine to study asthma.

## 2. Personalized Medicine through the Lens of Asthma

#### 1) What is Asthma?
A condition where a person's lungs become inflamed, and produce extra mucus, making it hard to breath. 

Biology behind asthma: An excessive allergen-induced type 2 inflammation, orchestrated by memory CD4+ T cells that produce type 2 cytokines (Th2 cells).

In a similar disease, rhinitis, its pathway also involves Th2 cells.

But unfortunately, there is currently no cure for asthma. Newer therapies are only partially successful in certain subtypes.

![asthma](https://github.com/miko-798/BENG_183_mini_lecture/blob/master/asthma.png)

> Thus we need to better understanding of the disease at a molecular level.

#### 2) A precision medicine study on asthma 

The figure below shows how scientists split the asthma patients into 4 subgroups. 

They took into account 8 parameters were correlated with their disease and the severity, and did a partition-around-medoids clustering.

![subgroups](https://github.com/miko-798/BENG_183_mini_lecture/blob/master/subgroups.png)

In the study, *Transcriptional profiling of Th2 cells identifies pathogenic features associated with asthma*, the researchers performed RNA-Seq in Th2 cells from a total of 80 samples from 77 patients including 3 biological replicates.

Then they did RNA-Seq analysis to identify genes differentially expressed between allergic asthma, rhinitis & healthy control groups, by performing negative binomial tests for pairwise comparisons employing the Bioconductor package DESeq2.

These are the findings:

- Identified a total of 15 distinct gene modules 
- DESeq analysis found 500 genes differentially expressed between asthmatic subjects and healthy subjects (Genes for apoptosis, zinc transporters, MAPK, NF-κB, TNF)
- Expression of most of these genes was similar between rhinitis and asthma
- Genes that differentiate asthmatic from healthy subjects show an intermediate phenotype in allergic rhinitis subjects

> These genetic markers identified through this study could offer insights for personalized medicine for asthma patients.

## 3. Current Hot Topics on Precision Medicine

> The study of precision medicine has gained an increased interest in the scientific community in the past decade. Some interesting work are presented as follows.

#### 1) Mapping of patients data

Atul Butte, a Distinguished Professor and the Director of the Computational Health Sciences Institute at UCSF, constructed a map illustrating how each individual patient developed different subtypes of diseases and how these diseases lead to mortality. 

Here is the map showing the paths of each patient:

Each square and circle represent a certain subtype of disease, and each line represents a transition. 

![map](https://github.com/miko-798/BENG_183_mini_lecture/blob/master/map.png)

This map offers physicians and scientists possible patterns of disease progression, which can help guide the treatments for future patients. This is one way to *build prediction models for clinical events based on electronic medical record (EMR) data*. The amount of detailed information encompassed by this map is powerful and grants possibility for precision care for patients.
 
> Let's look at another application of precision medicine.

#### 2) Opening the black box of machine learning models

Su-In Lee, an Associate Professor at Paul G. Allen School of Computer Science & Engineering at UW, found weaknesses in the conventional way to identify molecular markers. She tries to interpret the complex machine learning models that are used to analyze patient data, and strives to offer Individualized explanations for a particular prediction and for a particular patient. 

![su-in lee](https://github.com/miko-798/BENG_183_mini_lecture/blob/master/su-in%20lee.png)


> These are both very interesting and cutting edge research efforts in the field of precision medicine. So what's next in precision medicine? Well, let's keep in mind the three things that scientists need to address (at the beginning of chapter), and we all have the possibility of making what's next.


## References:
1. Seumois, Grégory et al. “Transcriptional Profiling of Th2 Cells Identifies Pathogenic Features Associated with Asthma” Journal of immunology (Baltimore, Md. : 1950) vol. 197,2 (2016): 655-64.
2. Su-In Lee Lab: https://suinlee.cs.washington.edu/research
3. Su-In Lee: "Interpretable Machine Learning for Precision Medicine" https://youtu.be/La7KTIe2DeU
4. Precisely practicing medicine with a trillion points of data. | Atul Butte | TEDxSanFrancisco https://www.youtube.com/watch?v=fbZZ_1Jbm6w












