# Taxosoft
_Taxosoft_
Taxosoft uses a combination of DBpedia and Word2vec trained on a domain specific corpus in order to generate synonyms and related terms for soft skills. More specifically, we train our word2vec model on a dataset of job ads provided by kaggle for salary prediction (https://www.kaggle.com/c/job-salary-prediction/data). Such method can be applied to other domains in order to extract synonyms domain specific, by training the word embeddings on a domain specific corpus.  
Also, it can be applied to other languages, for which DBpedia is rich enough.


_How to use_

```
From taxosoft import Alt_Words
model =  load your word embeddings model trained on a domain-specific corpus
word=input your word
rterms = Alt_Words(word, model)
print(rterms)
```

_References_

When using this code, please cite the following paper:

Imane Khaouja, Ghita Mezzour, Kathleen M. Carley, and Ismail Kassou. Building a Soft Skill Taxonomy from Job Openings. Social Network Analysis and Mining 9(1) 1:43, July 2019
```
@article{khaouja_building_2019,
	title = {Building a soft skill taxonomy from job openings},
	volume = {9},
	issn = {1869-5469},
	url = {https://doi.org/10.1007/s13278-019-0583-9},
	doi = {10.1007/s13278-019-0583-9},
	abstract = {Soft skills are crucial for candidates in the job market, and analyzing these skills listed in job ads can help in identifying the most important soft skills required by recruiters. This analysis can benefit from building a taxonomy to extract soft skills. However, most prior work is primarily focused on building hard skill taxonomies. Unfortunately, methodologies for building hard skill taxonomies do not work well for soft skills, due to the wide variety of terminologies used to list soft skills in job ads. Moreover, prior work has mainly focused on extracting soft skills from job ads using a simple keyword search, which can fail to detect the different forms in which soft skills are listed in job ads. In this paper, we develop TaxoSoft, a methodology for building a soft skill taxonomy that uses DBpedia and Word2Vec in order to find terms related to different soft skills. TaxoSoft also uses social network analysis to build a hierarchy of terms. We use this method to build soft skill taxonomies in both English and French. We evaluate TaxoSoft on a sample of job ads and find that it achieves an F-score of 0.84, while taxonomies developed in prior work achieve an F-score of only 0.54. We then use the proposed methodology to analyze soft skills listed in job ads in order to find the skills most required in the American and Moroccan job markets. Our findings can offer insights to universities about the top soft skills requested in the job market.},
	language = {en},
	number = {1},
	urldate = {2020-02-07},
	journal = {Social Network Analysis and Mining},
	author = {Khaouja, Imane and Mezzour, Ghita and Carley, Kathleen M. and Kassou, Ismail},
	month = aug,
	year = {2019},
	pages = {43}
}
```
