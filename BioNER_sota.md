# BioNER SOTA #

 An overview of the state-of-the-art (SOTA) across the most common BioNER tasks and their corresponding datasets.
 
- [Chemical NER](#1)
    -  CHEMDNER
    -  CDR-Chemical
- [Disease NER](#2)
    -  NCBI-Disease
    -  CDR-Disease
- [Gene/Protein NER](#3)
    -  BC2GM
    -  JNLPBA
- [Mutation NER](#4)
    -  MutationFinder
    -  tmVar
- [Species NER](#5)
    -  LINNAEUS


<h2 id="1">Chemical NER </h2>

### CHEMDNER  ### 
[CHEMDNER (chemical compound and drug name recognition) task](https://jcheminf.biomedcentral.com/articles/10.1186/1758-2946-7-S1-S1) as part of the BioCreative IV challenge aims to promote the development of systems for the automatic recognition of chemical entities in text. It was divided into two tasks: one covered the indexing of documents with chemicals (chemical document indexing - CDI task), and the other was concerned with finding the exact mentions of chemicals in text (chemical entity mention recognition - CEM task). Here, we only focus on the CEM task. 

The CHEMDNER corpus consists of 10,000 PubMed abstracts, which contains a total of 84,355 chemical entity mentions. The original corpus is divided into training set (3,500 abstracts), development set (3,500 abstracts) and test set (3,000 abstracts)

| Method | P | R | F1 | Paper | 
| ----------- | :----:| :----: | :----: | --- |
| tmChem (Leaman et al., 2015) | 89.09 | 85.75 | 87.39 | [tmChem: a high performance approach for chemical named entity recognition and normalization](https://jcheminf.biomedcentral.com/articles/10.1186/1758-2946-7-S1-S3)|
| CRF (Lu et al., 2015) | 88.73 | 87.41 | 88.06 | [CHEMDNER system with mixed conditional random fields and multi-scale word clustering](https://jcheminf.biomedcentral.com/articles/10.1186/1758-2946-7-S1-S4)|
| BiLSTM-CRF (Lample et al., 2016), Luo et al. (2018) rebuilt the model on the dataset | 91.31 | 87.73 | 89.48 | [Neural architectures for named entity recognition](https://arxiv.org/abs/1603.01360)|
| Att-BiLSTM-CRF (Luo et al., 2018) | 92.29 | 90.01 | 91.14 | [An attention-based BiLSTM-CRF approach to document-level chemical named entity recognition](https://academic.oup.com/bioinformatics/article/34/8/1381/4657076)|
| MTM-CW (Wang et al., 2019) | 91.30 | 87.53 | 89.37 | [Cross-type biomedical named entity recognition with deep multi-task learning](https://academic.oup.com/bioinformatics/article-abstract/35/10/1745/5126922?redirectedFrom=fulltext)|
| BioBERT (Lee et al., 2019) | 92.80 | 91.92 | 92.36 | [BioBERT: a pre-trained biomedical language representation model for biomedical text mining](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btz682/5566506?searchresult=1)|



### CDR-Chemical ###
[CDR (chemical disease relation) task](https://academic.oup.com/database/article/doi/10.1093/database/baw068/2630414) as part of the BioCreative V challenge aims to automatically extract CDRs from the literature. The CDR corpus consists of 1,500 PubMed abstracts with annotated chemicals, diseases and chemical-disease interactions, which contains a total of 15,933 chemical entity mentions. The original corpus is separated into training set (500 abstracts), development set (500 abstracts) and test set (500 abstracts). 

| Method | P | R | F1 | Paper | 
| ----------- | :----:| :----: | :----: | --- |
| TaggerOne (Leaman and Lu, 2016) | 94.20 | 88.80 | 91.40 | [TaggerOne: joint named entity recognition and normalization with semi-Markov Models](https://academic.oup.com/bioinformatics/article/32/18/2839/1744190)|
| BiLSTM-CRF (Lample et al., 2016), Luo et al. (2018) rebuilt the model on the dataset | 92.82 | 88.52 | 90.62 | [Neural architectures for named entity recognition](https://arxiv.org/abs/1603.01360)|
| Att-BiLSTM-CRF (Luo et al., 2018) | 93.49 | 91.68 | 92.57 | [An attention-based BiLSTM-CRF approach to document-level chemical named entity recognition](https://academic.oup.com/bioinformatics/article/34/8/1381/4657076)|
| D3NER (Dang et al., 2018) | 93.73 | 92.56 | 93.14 | [D3NER : biomedical named entity recognition using CRF-biLSTM improved with fine-tuned embeddings of various linguistic information](https://academic.oup.com/bioinformatics/article-abstract/34/20/3539/4990492)|
| CollaboNet (Yoon et al., 2018) | 94.26 | 92.38 | 93.31 | [CollaboNet: Collaboration of deep neural networks for biomedical named entity recognition](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2813-6)|
| ELMo (Peng et al., 2019) | - | - | 91.5 | [Transfer Learning in Biomedical Natural Language Processing: An Evaluation of BERT and ELMo on Ten Benchmarking Datasets](https://arxiv.org/abs/1906.05474)|
| BERT (Peng et al., 2019) | - | - | 93.5 | [Transfer Learning in Biomedical Natural Language Processing: An Evaluation of BERT and ELMo on Ten Benchmarking Datasets](https://arxiv.org/abs/1906.05474)|
| BioBERT (Lee et al., 2019) | 93.68 | 93.26 | 93.47 | [BioBERT: a pre-trained biomedical language representation model for biomedical text mining](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btz682/5566506?searchresult=1)|

</br>

<h2 id="2">Disease NER </h2>

### NCBI-Disease ###

The [NCBI Disease corpus](https://www.sciencedirect.com/science/article/pii/S1532046413001974) consists of 793 PubMed abstracts separated into training (593), development (100) and test (100) subsets. It contains a total of 6,892 disease entity mentions.

| Method | P | R | F1 | Paper | 
| ----------- | :----:| :----: | :----: | --- |
| DNorm (Leaman et al., 2015) | 82.2 | 77.5 | 79.8 | [DNorm: Disease name normalization with pairwise learning to rank](https://academic.oup.com/bioinformatics/article-abstract/29/22/2909/312804)|
| TaggerOne (Leaman and Lu, 2016) | 85.1 | 80.8 | 82.9 | [TaggerOne: joint named entity recognition and normalization with semi-Markov Models](https://academic.oup.com/bioinformatics/article/32/18/2839/1744190)|
| MCNN (Zhao et al., 2017) | 85.08 | 85.26 | 85.17 | [Disease named entity recognition from biomedical literature using a novel convolutional neural network](https://bmcmedgenomics.biomedcentral.com/articles/10.1186/s12920-017-0316-8)|
| BiLSTM-CRF (Lample et al., 2016), Wang et al. (2019) rebuilt the model on the dataset | 86.11 | 85.49 | 85.80 | [Neural architectures for named entity recognition](https://arxiv.org/abs/1603.01360)|
| CollaboNet (Yoon et al., 2018) | 85.61 | 82.61 | 84.08 | [CollaboNet: Collaboration of deep neural networks for biomedical named entity recognition](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2813-6)|
| GRAM-CNN (Zhu et al., 2018) | 86.46 | 88.07 | 87.26 | [GRAM-CNN: A deep learning approach with local context for named entity recognition in biomedical text](https://academic.oup.com/bioinformatics/article-abstract/34/9/1547/4764002)|
| MTM-CW (Wang et al., 2019) | 85.86 | 86.42 | 86.14 | [Cross-type biomedical named entity recognition with deep multi-task learning](https://academic.oup.com/bioinformatics/article-abstract/35/10/1745/5126922?redirectedFrom=fulltext)|
| Dic-Att-BiLSTM-CRF (Xu et al., 2019) | 88.3 | 89.0 | 88.6 | [Document-level attention-based BiLSTM-CRF incorporating disease dictionary for disease named entity recognition](https://www.sciencedirect.com/science/article/pii/S0010482519301106)|
| BioBERT (Lee et al., 2019) | 88.22 | 91.25 | 89.71 | [BioBERT: a pre-trained biomedical language representation model for biomedical text mining](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btz682/5566506?searchresult=1)|


### CDR-Disease ###
[CDR (chemical disease relation) task](https://academic.oup.com/database/article/doi/10.1093/database/baw068/2630414) as part of the BioCreative V challenge aims to automatically extract CDRs from the literature. The CDR corpus consists of 1,500 PubMed abstracts with annotated chemicals, diseases and chemical-disease interactions, which contains a total of 12,864 disease entity mentions. The original corpus is separated into training set (500 abstracts), development set (500 abstracts) and test set (500 abstracts). 


| Method | P | R | F1 | Paper | 
| ----------- | :----:| :----: | :----: | --- |
| HITSZ_CDR (Li et al., 2016) | 88.68 | 85.23 | 86.93 | [HITSZ_CDR: an end-to-end chemical and disease relation extraction system for BioCreative V](https://academic.oup.com/database/article-abstract/doi/10.1093/database/baw077/2630439)|
| TaggerOne (Leaman and Lu, 2016) | 85.2 | 80.2 | 82.6 | [TaggerOne: joint named entity recognition and normalization with semi-Markov Models](https://academic.oup.com/bioinformatics/article/32/18/2839/1744190)|
| BiLSTM-CRF (Lample et al., 2016), Wang et al. (2019) rebuilt the model on the dataset | 87.60 | 86.25 | 86.92 | [Neural architectures for named entity recognition](https://arxiv.org/abs/1603.01360)|
| MCNN (Zhao et al., 2017) | 88.20 | 87.46 | 87.83 | [Disease named entity recognition from biomedical literature using a novel convolutional neural network](https://bmcmedgenomics.biomedcentral.com/articles/10.1186/s12920-017-0316-8)|
| Transition-based joint model (Lou et al., 2017) | 89.61 | 83.09 | 86.23 | [A Transition-based Joint Model for Disease Named Entity Recognition and Normalization](https://academic.oup.com/bioinformatics/article-abstract/33/15/2363/3089942)|
| CollaboNet (Yoon et al., 2018) | 85.61 | 82.61 | 84.08 | [CollaboNet: Collaboration of deep neural networks for biomedical named entity recognition](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2813-6)|
| MTM-CW (Wang et al., 2019) | 89.10 | 88.47 | 88.78 | [Cross-type biomedical named entity recognition with deep multi-task learning](https://academic.oup.com/bioinformatics/article-abstract/35/10/1745/5126922?redirectedFrom=fulltext)|
| Dic-Att-BiLSTM-CRF (Xu et al., 2019) | 89.1 | 87.5 | 88.3 | [Document-level attention-based BiLSTM-CRF incorporating disease dictionary for disease named entity recognition](https://www.sciencedirect.com/science/article/pii/S0010482519301106)|
| BERT (Peng et al., 2019) | - | - | 86.6 | [Transfer Learning in Biomedical Natural Language Processing: An Evaluation of BERT and ELMo on Ten Benchmarking Datasets](https://arxiv.org/abs/1906.05474)|
| BioBERT (Lee et al., 2019) | 86.47 | 87.84 | 87.15 | [BioBERT: a pre-trained biomedical language representation model for biomedical text mining](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btz682/5566506?searchresult=1)|


</br>

<h2 id="3">Gene/Protein NER </h2>


### BC2GM ###
[Gene Mention Tagging task](https://genomebiology.biomedcentral.com/articles/10.1186/gb-2008-9-s2-s2) as part of the BioCreative II challenge is concerned with the named entity extraction of gene and gene product mentions in text. The BC2GM corpus contains a total of 24,583 gene entity mentions. 

| Method | P | R | F1 | Paper | 
| ----------- | :----:| :----: | :----: | --- |
| BiLSTM-CRF (Lample et al., 2016), Wang et al. (2019) rebuilt the model on the dataset | 81.57 | 79.48 | 80.51 | [Neural architectures for named entity recognition](https://arxiv.org/abs/1603.01360)|
| CollaboNet (Yoon et al., 2018) | 80.49 | 78.99 | 79.73 | [CollaboNet: Collaboration of deep neural networks for biomedical named entity recognition](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2813-6)|
| BiLM-NER (Sachan et al., 2018) | 81.81 | 81.57 | 81.69 | [Effective Use of Bidirectional Language Modeling for Transfer Learning in Biomedical Named Entity Recognition](http://proceedings.mlr.press/v85/sachan18a.html)|
| MTM-CW (Wang et al., 2019) | 82.10 | 79.42 | 80.74 | [Cross-type biomedical named entity recognition with deep multi-task learning](https://academic.oup.com/bioinformatics/article-abstract/35/10/1745/5126922?redirectedFrom=fulltext)|
| BioBERT (Lee et al., 2019) | 84.32 | 85.12 | 84.72 | [BioBERT: a pre-trained biomedical language representation model for biomedical text mining](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btz682/5566506?searchresult=1)|


### JNLPBA ###
[JNLPBA corpus](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.122.8012&rep=rep1&type=pdf#page=83) contains 2,404 abstracts extracted from MEDLINE using the MeSH terms “human”, “blood- cell” and “transcription factor”. The manual annotation of these abstracts was based on five classes of the GENIA ontology, namely protein, DNA, RNA, cell line, and cell type. This corpus was used in the Bio-Entity Recognition Task in BioNLP/NLPBA 2004, providing 2,000 abstracts for training and the remaining 404 abstracts for testing. The overall results are shown in the following table.

| Method | P | R | F1 | Paper | 
| ----------- | :----:| :----: | :----: | --- |
| SVM (Zhou and Su., 2004) | 69.42 | 75.99 | 72.55 | [Exploring Deep Knowledge Resources in Biomedical Name Recognition](https://dl.acm.org/citation.cfm?id=1567616)|
| CRF_NERBio (Tsai et al., 2006) | 72.01 | 73.98 | 72.98 | [NERBio: using selected word conjunctions, term normalization, and global patterns to improve biomedical named entity recognition](https://bmcbioinformatics.biomedcentral.com/track/pdf/10.1186/1471-2105-7-S5-S11)|
| BiLSTM-CRF (Lample et al., 2016), Wang et al. (2019) rebuilt the model on the dataset | 71.35 | 75.74 | 73.48 | [Neural architectures for named entity recognition](https://arxiv.org/abs/1603.01360)|
| BiLM-NER (Sachan et al., 2018) | 71.39 | 79.06 | 75.03 | [Effective Use of Bidirectional Language Modeling for Transfer Learning in Biomedical Named Entity Recognition](http://proceedings.mlr.press/v85/sachan18a.html)|
| CollaboNet (Yoon et al., 2018) | 74.43 | 83.22 | 78.58 | [CollaboNet: Collaboration of deep neural networks for biomedical named entity recognition](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2813-6)|
| MTM-CW (Wang et al., 2019) | 70.91 | 76.34 | 73.52 | [Cross-type biomedical named entity recognition with deep multi-task learning](https://academic.oup.com/bioinformatics/article-abstract/35/10/1745/5126922?redirectedFrom=fulltext)|
| BioBERT (Lee et al., 2019) | 72.24 | 83.56 | 77.49 | [BioBERT: a pre-trained biomedical language representation model for biomedical text mining](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btz682/5566506?searchresult=1)|


</br>

<h2 id="4">Mutation NER </h2>

### MuatationFinder corpus  and tmVar corpus ###

[The MutationFinder corpus](https://academic.oup.com/bioinformatics/article-abstract/23/14/1862/188647) was established to guide the construction of the patterns. The development data set is made up of 605 point mutation mentions in 305 abstracts selected randomly from primary citations in PDB. The evaluation data set is made up of 910 point mutation mentions in 508 abstracts annotated by two of the authors, not involved in the development of the system.

[The tmVar corpus](https://academic.oup.com/bioinformatics/article-abstract/29/11/1433/220291) comprises 500 abstracts manually annotated from which 334 were used for training tmVar while the remaining 166 were used for testing it. 

| Method | MF-P | MF-R | MF-F1 | tmvar-P | tmvar-R | tmvar-F1 |Paper | 
| ----------- | :----:| :----: | :----: |:----:| :----: | :----: | --- |
| MutationFinder (Caporaso et al., 2007) | 98.41 | 81.92 | 89.41 | 89.66 | 69.15 | 78.08 | [MutationFinder: A high-performance system for extracting point mutation mentions from text](https://academic.oup.com/bioinformatics/article-abstract/23/14/1862/188647)|
| tmVar (Wei et al., 2013) | 98.80 | 89.62 | 93.98 | 91.38 | 91.40 | 91.39 | [tmVar: a text mining approach for extracting sequence variants in biomedical literature](https://academic.oup.com/bioinformatics/article-abstract/29/11/1433/220291)|
| SETH (Thomas et al., 2016) | 98 | 82 | 89 | 95 | 77 | 85 | [SETH detects and normalizes genetic variants in text](https://academic.oup.com/bioinformatics/article/32/18/2883/1743171)|
| Character-based network (Thomas et al., 2018) | - | - | - | 88.1 | 86.6 | 87.4 | [Recognition of genetic mutations in text using Deep Learning](https://dl.acm.org/citation.cfm?id=3280020)|

</br>

<h2 id="5">Species NER </h2>


### LINNAEUS corpus ###

[The LINNAEUS corpus](https://academic.oup.com/bioinformatics/article-abstract/23/14/1862/188647): A set of open access documents in text format, manually annotated for species mention tags. It consists of 100 full-text documents from the PMC OA document, which contains a total of 4,259 species entity mentions.

| Method | P | R | F1 | Paper | 
| ----------- | :----:| :----: | :----: | --- |
| LINNAEUS (Gerner et al., 2010) | 97.07 | 94.28 | 95.65 | [LINNAEUS : A species name identification system for biomedical literature](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-11-85)|
| SR4GN (Wei et al., 2012) | 86 | 85 | 86 | [SR4GN : A Species Recognition Software Tool for Gene Normalization](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0038460)|
| BiLSTM-CRF (Habibi et al., 2017) | - | - | 94.03 | [Deep learning with word embeddings improves biomedical named entity recognition](https://academic.oup.com/bioinformatics/article/33/14/i37/3953940#118768624)|
| Transfer learning-based model (Giorgi and Bader, 2018) | 92.80 | 94.29 | 93.54 | [Transfer learning for biomedical named entity recognition with neural networks](https://academic.oup.com/bioinformatics/article-abstract/34/23/4087/5026661)|
| BioBERT (Lee et al., 2019) | 93.84 | 86.11 | 89.81 | [BioBERT: a pre-trained biomedical language representation model for biomedical text mining](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btz682/5566506?searchresult=1)|
