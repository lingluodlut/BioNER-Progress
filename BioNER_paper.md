# BioNER Papers #

A paper list for BioNER

Over the past decades, many automatic BioNER methods have been proposed and used to recognise biomeidcal entities. They can be categorised into dictionary-based, rule-based and machine learning-based methods. Recently, neural network-based machine learning methods exhibit promising results.

![image](/image/trend.png)

## Survey Papers ##
1. **Overview of BioCreative II gene mention recognition**. Smith L, Tanabe L K, nee Ando R J, et al. *Genome biology*, 2008, 9(2): S2. [[paper]](https://genomebiology.biomedcentral.com/articles/10.1186/gb-2008-9-s2-s2)
2. **Biomedical named entity recognition: a survey of machine-learning tools**. Campos D, Matos S, Oliveira J L. *Theory and Applications for Advanced Text Mining*, 2012: 175-195. [[paper]](https://books.google.com.hk/books?hl=zh-CN&lr=&id=EfqdDwAAQBAJ&oi=fnd&pg=PA175&ots=WEKIblRekC&sig=FWoufJtWVSDHD3gbWaZXruEOiEs&redir_esc=y#v=onepage&q&f=false)
2. **Chemical named entities recognition: a review on approaches and applications**.  Eltyeb S, Salim N. *Journal of cheminformatics*, 2014, 6(1): 17. [[paper]](https://jcheminf.biomedcentral.com/articles/10.1186/1758-2946-6-17)
3. **CHEMDNER: The drugs and chemical names extraction challenge**. Krallinger M, Leitner F, Rabal O, et al. *Journal of cheminformatics*, 2015, 7(1): S1. [[paper]](https://jcheminf.biomedcentral.com/articles/10.1186/1758-2946-7-S1-S1)
4. **A comparative study for biomedical named entity recognition**. Wang X, Yang C, Guan R. *International Journal of Machine Learning and Cybernetics*, 2015, 9(3): 373-382. [[paper]](https://link.springer.com/article/10.1007/s13042-015-0426-6)

## Dictionary-based Methods ##
1. **Using BLAST for identifying gene and protein names in journal articles**. Krauthammer M, Rzhetsky A, Morozov P, et al. *Gene*, 2000, 259(1-2): 245-252. [[paper]](https://www.sciencedirect.com/science/article/pii/S0378111900004315)
2. **Boosting precision and recall of dictionary-based protein name recognition**. Tsuruoka Y, Tsujii J. *Proceedings of the ACL 2003 workshop on Natural language processing in biomedicine-Volume 13*, 2003: 41-48. [[paper]](https://aclanthology.info/pdf/W/W03/W03-1306.pdf)
2. **Exploiting the performance of dictionary-based bio-entity name recognition in biomedical literature**. Yang Z, Lin H, Li Y. *Computational Biology and Chemistry*, 2008, 32(4): 287-291. [[paper]](https://www.sciencedirect.com/science/article/pii/S1476927108000340)
2. **A dictionary to identify small molecules and drugs in free text**. Hettne K M, Stierum R H, Schuemie M J, et al. *Bioinformatics*, 2009, 25(22): 2983-2991. [[paper]](https://academic.oup.com/bioinformatics/article-abstract/25/22/2983/180399) [[dictionary]](https://biosemantics.org/index.php/resources/jochem)
3. **LINNAEUS: a species name identification system for biomedical literature**. Gerner M, Nenadic G, Bergman C M. *BMC bioinformatics*, 2010, 11(1): 85. [[paper]](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-11-85)

## Rule-based Methods ##
1. **Toward information extraction: identifying protein names from biological papers**. Fukuda K, Tsunoda T, Tamura A, et al. *Pac symp biocomput*. 1998, 707(18): 707-718. [[paper]](https://pdfs.semanticscholar.org/335e/8b19ea50d3af6fcefe6f8421e2c9c8936f3f.pdf)
2. **A biological named entity recognizer**. Narayanaswamy M, Ravikumar K E, Vijay-Shanker K. *Biocomputing* 2003. 2002: 427-438. [[paper]](https://www.worldscientific.com/doi/abs/10.1142/9789812776303_0040)
3. **ProMiner: rule-based protein and gene entity recognition**. Hanisch D, Fundel K, Mevissen H T, et al. *BMC bioinformatics*, 2005, 6(1): S14. [[paper]](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-6-S1-S14)
4. **MutationFinder: a high-performance system for extracting point mutation mentions from text**. Caporaso J G, Baumgartner Jr W A, Randolph D A, et al. *Bioinformatics*, 2007, 23(14): 1862-1865. [[paper]](https://academic.oup.com/bioinformatics/article/23/14/1862/188647) [[code]](http://mutationfinder.sourceforge.net/)
3. **Drug name recognition and classification in biomedical texts: a case study outlining approaches underpinning automated systems**. Segura-Bedmar I, Martínez P, Segura-Bedmar M.  *Drug discovery today*, 2008, 13(17-18): 816-823. [[paper]](https://www.sciencedirect.com/science/article/pii/S1359644608002171)
3. **Investigation of unsupervised pattern learning techniques for bootstrap construction of a medical treatment lexicon**. Xu R, Morgan A, Das A K, et al. *Proceedings of the workshop on current trends in biomedical natural language processing*, 2009: 63-70. [[paper]](http://www.aclweb.org/anthology/W09-1308)
4. **Linguistic approach for identification of medication names and related information in clinical narratives**.  Hamon T, Grabar N. *Journal of the American Medical Informatics Association*, 2010, 17(5): 549-554. [[paper]](https://academic.oup.com/jamia/article/17/5/549/831598)
5. **SETH detects and normalizes genetic variants in text**. Thomas P, Rocktäschel T, Hakenberg J, et al. *Bioinformatics*, 2016, 32(18): 2883-2885. [[paper]](https://academic.oup.com/bioinformatics/article/32/18/2883/1743171) [[code]](http://rockt.github.io/SETH/)
5. **PENNER: Pattern-enhanced Nested Named Entity Recognition in Biomedical Literature**. Wang X, Zhang Y, Li Q, et al. *2018 IEEE International Conference on Bioinformatics and Biomedicine (BIBM)*. 2018: 540-547. [[paper]](https://ieeexplore.ieee.org/abstract/document/8621485/)


## Machine Learning-based Methods  ##

### SVM-based Methods ###
1. **Tuning support vector machines for biomedical named entity recognition**. Kazama J, Makino T, Ohta Y, et al. *Proceedings of the ACL-02 workshop on Natural language processing in the biomedical domain-Volume 3*, 2002: 1-8. [[paper]](https://aclanthology.info/pdf/W/W02/W02-0301.pdf)
2. **Biomedical named entity recognition using two-phase model based on SVMs**. Lee K J, Hwang Y S, Kim S, et al. *Journal of Biomedical Informatics*, 2004, 37(6): 436-447. [[paper]](https://www.sciencedirect.com/science/article/pii/S1532046404000863)
3. **Exploring deep knowledge resources in biomedical name recognition**. GuoDong Z, Jian S. *Proceedings of the International Joint Workshop on Natural Language Processing in Biomedicine and its Applications*, 2004: 96-99. [[paper]](https://aclanthology.info/pdf/W/W04/W04-1219.pdf)

### HMM-based Methods ###
1. **Named entity recognition in biomedical texts using an HMM model**. Zhao S. *Proceedings of the International Joint Workshop on Natural Language Processing in Biomedicine and its Applications*, 2004: 84-87.[[paper]](https://aclanthology.info/pdf/W/W04/W04-1216.pdf)
2. **Annotation of chemical named entities**. Corbett P, Batchelor C, Teufel S. P*roceedings of the Workshop on BioNLP 2007: Biological, Translational, and Clinical Language Processing*, 2007: 57-64. [[paper]](https://aclanthology.info/pdf/W/W07/W07-1008.pdf)
1. **Conditional random fields vs. hidden markov models in a biomedical named entity recognition task**. Ponomareva N, Rosso P, Pla F, et al. *Proc. of Int. Conf. Recent Advances in Natural Language Processing, RANLP*. 2007, 479: 483.[[paper]](http://clg.wlv.ac.uk/papers/Ponomareva-RANLP-07.pdf)

### MEMM-based Mehtods ###
1. **Cascaded classifiers for confidence-based chemical named entity recognition**. Corbett P, Copestake A. *BMC bioinformatics*, 2008, 9(11): S4. [[paper]](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-9-S11-S4)
2. **OSCAR4: a flexible architecture for chemical text-mining**. Jessop D M, Adams S E, Willighagen E L, et al. *Journal of cheminformatics*, 2011, 3(1): 41. [[paper]](https://jcheminf.biomedcentral.com/articles/10.1186/1758-2946-3-41)

### CRF-based Methods ###
1. **ABNER: an open source tool for automatically tagging genes, proteins and other entity names in text**. Settles B. *Bioinformatics*, 2005, 21(14): 3191-3192.[[paper]](https://academic.oup.com/bioinformatics/article/21/14/3191/266815)
2.  **BANNER: an executable survey of advances in biomedical named entity recognition**. Leaman R, Gonzalez G. *Biocomputing* 2008. 2008: 652-663.[[paper]](https://psb.stanford.edu/psb-online/proceedings/psb08/leaman.pdf)
3.  **Detection of IUPAC and IUPAC-like chemical names**. Klinger R, Kolářik C, Fluck J, et al. *Bioinformatics*, 2008, 24(13): i268-i276. [[paper]](https://academic.oup.com/bioinformatics/article-abstract/24/13/i268/235854)
3.  **Incorporating rich background knowledge for gene named entity classification and recognition**. Li Y, Lin H, Yang Z. *BMC bioinformatics*, 2009, 10(1): 223. [[paper]](https://bmcbioinformatics.biomedcentral.com/track/pdf/10.1186/1471-2105-10-223)
3.  **A study of machine-learning-based approaches to extract clinical entities and their assertions from discharge summaries**. Jiang M, Chen Y, Liu M, et al. *Journal of the American Medical Informatics Association*, 2011, 18(5): 601-606. [[paper]](https://academic.oup.com/jamia/article/18/5/601/834186)
4.   **ChemSpot: a hybrid system for chemical named entity recognition**. Rocktäschel T, Weidlich M, Leser U. *Bioinformatics*, 2012, 28(12): 1633-1640. [[paper]](https://academic.oup.com/bioinformatics/article/28/12/1633/266861)
3.  **Gimli: open source and high-performance biomedical name recognition**. Campos D, Matos S, Oliveira J L. *BMC bioinformatics*, 2013, 14(1): 54. [[paper]](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-14-54)
4.  **tmVar: a text mining approach for extracting sequence variants in biomedical literature**. Wei C H, Harris B R, Kao H Y, et al. *Bioinformatics*, 2013, 29(11): 1433-1439. [[paper]](https://academic.oup.com/bioinformatics/article-abstract/29/11/1433/220291) [[code]](https://www.ncbi.nlm.nih.gov/research/bionlp/Tools/tmvar/)
4.  **Evaluating word representation features in biomedical named entity recognition tasks**. Tang B, Cao H, Wang X, et al. *BioMed research international*, 2014, 2014. [[paper]](http://downloads.hindawi.com/journals/bmri/2014/240403.pdf)
5.  **Drug name recognition in biomedical texts: a machine-learning-based method**. He L, Yang Z, Lin H, et al. *Drug discovery today*, 2014, 19(5): 610-617. [[paper]](https://www.sciencedirect.com/science/article/pii/S1359644613003322)
3.  **tmChem: a high performance approach for chemical named entity recognition and normalization**. Leaman R, Wei C H, Lu Z. *Journal of cheminformatics*, 2015, 7(1): S3. [[paper]](https://jcheminf.biomedcentral.com/articles/10.1186/1758-2946-7-S1-S3)
4.  **GNormPlus: an integrative approach for tagging genes, gene families, and protein domains**. Wei C H, Kao H Y, Lu Z. *BioMed research international*, 2015, 2015. [[paper]](http://downloads.hindawi.com/journals/bmri/2015/918710.pdf)
5.  **Mining chemical patents with an ensemble of open systems**[J]. Leaman R, Wei C H, Zou C, et al. *Database*, 2016, 2016. [[paper]](https://academic.oup.com/database/article-abstract/doi/10.1093/database/baw065/2630406)
6. **nala: text mining natural language mutation mentions**.  Cejuela J M, Bojchevski A, Uhlig C, et al. *Bioinformatics*, 2017, 33(12): 1852-1858. [[paper]](https://academic.oup.com/bioinformatics/article-abstract/33/12/1852/2991428)


### Neural Network-based Methods ###
1. **Recurrent neural network models for disease name recognition using domain invariant features**. Sahu S, Anand A. *Proceedings of the 54th Annual Meeting of the Association for Computational Linguistics*. 2016: 2216-2225. [[paper]](https://www.aclweb.org/anthology/P16-1209)
2. **Deep learning with word embeddings improves biomedical named entity recognition**. Habibi M, Weber L, Neves M, et al. *Bioinformatics*, 2017, 33(14): i37-i48. [[paper]](https://academic.oup.com/bioinformatics/article/33/14/i37/3953940)
3.  **A neural joint model for entity and relation extraction from biomedical text**. Li F, Zhang M, Fu G, et al. *BMC bioinformatics*, 2017, 18(1): 198. [[paper]](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-017-1609-9)
2. **A neural network multi-task learning approach to biomedical named entity recognition**. Crichton G, Pyysalo S, Chiu B, et al. *BMC bioinformatics*, 2017, 18(1): 368. [[paper]](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-017-1776-8) [[code]](https://github.com/cambridgeltl/MTL-Bioinformatics-2016)
3. **Disease named entity recognition from biomedical literature using a novel convolutional neural network**. Zhao Z, Yang Z, Luo L, et al. *BMC medical genomics*, 2017, 10(5): 73. [[paper]](https://bmcmedgenomics.biomedcentral.com/articles/10.1186/s12920-017-0316-8)
3. **An attention-based BiLSTM-CRF approach to document-level chemical named entity recognition**. Luo L, Yang Z, Yang P, et al. *Bioinformatics*, 2018, 34(8): 1381-1388. [[paper]](https://academic.oup.com/bioinformatics/article-abstract/34/8/1381/4657076) [[code]](https://github.com/lingluodlut/Att-ChemdNER)
4. **GRAM-CNN: a deep learning approach with local context for named entity recognition in biomedical text**.  Zhu Q, Li X, Conesa A, et al. *Bioinformatics*, 2018, 34(9): 1547-1554. [[paper]](https://academic.oup.com/bioinformatics/article-abstract/34/9/1547/4764002) [[code]](https://github.com/valdersoul/GRAM-CNN)
4. **D3NER: biomedical named entity recognition using CRF-biLSTM improved with fine-tuned embeddings of various linguistic information**. Dang T H, Le H Q, Nguyen T M, et al. *Bioinformatics*, 2018, 34(20): 3539-3546. [[paper]](https://academic.oup.com/bioinformatics/article/34/20/3539/4990492) [[code]](https://github.com/aidantee/D3NER)
4. **Transfer learning for biomedical named entity recognition with neural networks**. Giorgi J M, Bader G D. *Bioinformatics*, 2018, 34(23): 4087-4094. [[paper]](https://academic.oup.com/bioinformatics/article/34/23/4087/5026661)
5. **Label-Aware Double Transfer Learning for Cross-Specialty Medical Named Entity Recognition**. Wang Z, Qu Y, Chen L, et al. *NAACL*. 2018: 1-15. [[paper]](https://www.aclweb.org/anthology/N18-1001)
6. **Recognizing irregular entities in biomedical text via deep neural networks**. Li F, Zhang M, Tian B, et al. *Pattern Recognition Letters*, 2018, 105: 105-113. [[paper]](https://www.sciencedirect.com/science/article/pii/S0167865517302155)
2. **Cross-type biomedical named entity recognition with deep multi-task learning**. Wang X, Zhang Y, Ren X, et al. *Bioinformatics*, 2019, 35(10): 1745-1752. [[paper]](https://academic.oup.com/bioinformatics/article/35/10/1745/5126922) [[code]](https://github.com/yuzhimanhua/lm-lstm-crf) 
3. **Improving Chemical Named Entity Recognition in Patents with Contextualized Word Embeddings**.  Zhai Z, Nguyen D Q, Akhondi S, et al. *Proceedings of the 18th BioNLP Workshop and Shared Task*. 2019: 328-338. [[paper]](https://www.aclweb.org/anthology/W19-5035) [[code]](https://github.com/zenanz/ChemPatentEmbeddings)
4. **Chinese Clinical Named Entity Recognition Using Residual Dilated Convolutional Neural Network with Conditional Random Field**. Qiu J, Zhou Y, Wang Q, et al. *IEEE Transactions on NanoBioscience*, 2019, 18(3): 306-315. [[paper]](https://ieeexplore.ieee.org/abstract/document/8678833/)
5. **A Neural Multi-Task Learning Framework to Jointly Model Medical Named Entity Recognition and Normalization**. Zhao S, Liu T, Zhao S, et al. *Proceedings of the AAAI Conference on Artificial Intelligence*. 2019, 33: 817-824. [[paper]](https://wvvw.aaai.org/ojs/index.php/AAAI/article/download/3861/3739)
6. **CollaboNet: collaboration of deep neural networks for biomedical named entity recognition**. Yoon W, So C H, Lee J, et al. *BMC bioinformatics*, 2019, 20(10): 249. [[paper]](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2813-6) [[code]](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2813-6)
6. **BioBERT: a pre-trained biomedical language representation model for biomedical text mining**. Lee J, Yoon W, Kim S, et al. *Bioinformatics*, Advance article, 2019. [[paper]](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btz682/5566506) [[code]](https://github.com/dmis-lab/biobert)
7. **HUNER: Improving Biomedical NER with Pretraining**. Weber L, Münchmeyer J, Rocktäschel T, et al. *Bioinformatics*, Advance article, 2019. [[paper]](https://academic.oup.com/bioinformatics/advance-article-abstract/doi/10.1093/bioinformatics/btz528/5523847?redirectedFrom=fulltext) [[code]](https://hu-ner.github.io/)
### Others ###
1. **TaggerOne: joint named entity recognition and normalization with semi-Markov Models**. Leaman R, Lu Z. *Bioinformatics*, 2016, 32(18): 2839-2846. [[paper]](https://academic.oup.com/bioinformatics/article/32/18/2839/1744190) [[code]](https://www.ncbi.nlm.nih.gov/research/bionlp/tools/taggerone/)
2. **A transition-based joint model for disease named entity recognition and normalization**. Lou Y, Zhang Y, Qian T, et al. *Bioinformatics*, 2017, 33(15): 2363-2371. [[paper]](https://academic.oup.com/bioinformatics/article-abstract/33/15/2363/3089942) [[code]](https://github.com/louyinxia/jointRN)



