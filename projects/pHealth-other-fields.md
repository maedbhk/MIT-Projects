---
title: pHealth in other fields
---

> Much of the points below came from a [review paper](https://pubmed.ncbi.nlm.nih.gov/33091314/) by MacEachern and Forkert (2020)

## Examples of pHealth in practice
* One of the first fields to use a precision medicine approach to treat human disease was transfusion medicine, where the discovery of blood types in the early 1900s revolutionized blood transfusions, allowing for matching of donor and recipient blood types, and avoiding complications associated with mismatched donor and recipient blood [Giangrande et al. 2000](https://onlinelibrary.wiley.com/doi/full/10.1046/j.1365-2141.2000.02139.x)
* pHealth has enabled gene therapy for infants with spinal muscular atrophy (SMA) type I

## Genetics, genomics and pHealth
* Genetics is the study of genes and their roles in inheritance 
* Genomics is the study of a person's genome and the interactions within the genome and the greater environment
* Other fields now incorporate their data in pHealth:
    * epigenetics, proteomics (protein), metabolomics (metabolics), radiomics (radiology), pharmacomics (pharmacology), microbiomics (microbiome)
* Multi-omics: inclusion of data from multiple domains

## Machine learning
* Machine learning is a branch of artificial intelligence in which computer-based models are created to learn and identify patterns in 
high dimensional datasets to create prediction and classification models based on training data
* ML is typically divided into supervised, unsupervised and reinforcement learning (RL)
* In pHealth, supervised and unsupervised approaches are more common than RL, since the latter requires direct feedback 

## Unsupervised/supervised learning?
* Unsupervised learning aims to uncover patterns in unlabelled data - in doing so, it can automatically identify clusters of similar cases within a dataset (e.g., variational autoencoders, k-means, pca)
* Supervised learning aims to identify patterns in multi-dimensional data based on labelled data (e.g., healthy vs disease). A training dataset with ground truth labels is typically used
to build a model and optimize performance of the ML model for the desired outcome. The uncovered (learned) patterns can then be used to classify new datasets or make data-driven, patient-individual predictions. Some popular supervised learning approaches: SVM, random forests, linear models, deep neural nets.

## Artificial neural networks
* basic make-up: input layer, multiple hidden layers, output layer
* number of "neurons" in the input layer is equal to the number of input features while the number of "neurons" in the output layer is equal to the number of classes in case of a classification problem (e.g., patients with/without a disease)
* Artificial neural networks with many hidden layers are typically referred to as deep neural networks. 
* Convolutional neural networks apply convolutional filters in the first layers of the deep neural network that can automatically identify important temporal or spatial features in a dataset such as three-dimensional imaging data. Convolutional filters are optimized in the same fashion as network weights are optimized. 

## ML and pHealth
* Certain conditions should be met in order for ML approaches to be useful for pHealth
    * input data must be high quality with small artifact or noise levels
    * ground truth labels must be correct (e.g., correct diagnosis/diagnostic labels)
    * training set without missing features
    * large datasets which enable the models to learn the true variation in the data with reduced risk that a few outliers affect the model negatively
    * in classification for pHealth, both precision and accuracy are important and should both be optimized

## Advantages and limitations of ML for pHealth
* advantages:
    * no strict assumption about data distribution (models can combine multi-omics data)
    * regularization is widely used in ML models, therefore, these models can usually handle noisy data and large variances
    * complex ML models have the ability to identify multi-faceted, non-linear patterns in training data, which might not be observable to simple linear models
* limitations:
    * the ability to identify non-linear patterns comes with reduced interpretation capabilities, compared to simple linear models (i.e. black box criticism)
    * in overfitting training data, models often fail to generalize, this happens more often with complex models. deep neural networks with thousands (millions) of features often fail to generalize

## ML and genomics
* GWAS studies (genome-wide association studies): genomic information is examined to identify variants associated with a trait or phenotype. some work has shown that genotype-based disease risk assessment may be possible for diseases for which single nucleotide polymorphism (SNP) arrays carry a large risk proportion
* ML models can also be applied to multi-modal data acquired through electronic medical records (EMRs) to identify patients with conditions that may benefit from early treatment or participation in randomized control trials or novel interventions. 