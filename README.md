# Gene-to-Phenotype Predictions

## Introduction

A major question in biomedical research is how genes map to phenotypes (i.e., which genes influence which phenotypes of an organism). Large-scale empirical efforts have been underway for quite some time, for instance with the goal to measure the functional consequences of gene knockouts in mice. The International Mouse Phenotyping Consortium (IMPC) is, along those lines, collecting hundreds of phenotypes in mouse lines that carry single-gene knockouts to facilitate gene-to-phenotype mappings. However, despite immense effort and resources invested, there is currently only limited information available. For instance, even for the most densely covered phenotypes, data are available for approx. only 1/3 of the genes existing in the mouse genome. Hence, there would be substantive value to approaches that expedite the endeavor of gene-to-phenotype mapping. Here, we would like to explore whether computational approaches could be used to accurately predict phenotypic outcome resulting from a given gene knockout.

As an initial proof-of-principle, in the context of IMPC data, we attempted to predict phenotype based on genotype (i.e., whether a given gene is knocked out or not) for only one specific phenotype: body weight. Towards this end, we built a range of models that accept as input some information about the gene that’s being knocked out (more on that below) and output the predicted effect that this gene is going to have on body weight.

Our modelling efforts were organized in 3 work packages (WP). In the context of WP1, we obtained multi-level gene features sets that link genes to features in different levels of biological organization, ranging from genes to proteins, cells, tissues and organismal phenotypes. We used various regressors, classifiers and graph convolutional networks to predict body weight effects based on these feature sets. WP2, in contrast, focused on DNA sequence and protein structural features to address whether body weight effects can be predict based on data from these levels of biological organization. Towards this end, we used a DNA language model as well as convolutional neural networks combined with protein sequence data. In WP3, we pursued a complementary approach to the analysis of DNA- and protein-sequence-centered modelling efforts. Specifically, we used TF-IDF vectorization of DNA and protein sequence data to obtain features for body weight effect size prediction.

Three GitHub projects comprise the codebase for the Gene-to-Phenotype Precitions project. Each project consists of a GitHub repository that contains its code and a Google Drive link that contains its source data and its results.

## Multi-level Gene Feature-based Phenotype Prediction (WP1)

- [code](https://github.com/gene-to-phenotype-predictions/ehninger)
- [data](https://drive.google.com/drive/folders/1z2tPAdBlrSsVvAuO5ICsRmbGRBLbeSnd)

## Machine Learning Phenotype Prediction (WP2)

- [code](https://github.com/gene-to-phenotype-predictions/bert_dna_weight)
- [data](https://drive.google.com/drive/folders/1Exv-jo6RlcHdD5fPYqSA0v3TN0FGducF?usp=sharing)

## Baseline TF-IDF Analysis (WP3)

- [code](https://github.com/gene-to-phenotype-predictions/adpatter)
- [data](https://drive.google.com/drive/folders/1a-uW8QXx_auK52q9y1cJm1uMr3DYLlBo?usp=sharing)
