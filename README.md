# PTM

The implementation of Prescription Topic Model in our paper:

Liang Yao, Yin Zhang, Baogang Wei, Wenjin Zhang, Zhe Jin. "A Topic Modeling Approach for Traditional Chinese Medicine Prescriptions". IEEE Transactions on Knowledge and Data Engineering (TKDE), 2018. DOI:10.1109/TKDE.2017.2787158

# Require
Java 7 or above, I use Java 8 in this project.

Eclipse


# Data

All 33,765 prescriptions: /file/pre_herbs.txt, file/pre_symptoms.txt. 

Training set: /file/pre_herbs_train.txt, /file/pre_symptoms_train.txt

Test set: /file/pre_herbs_test.txt, /file/pre_symptoms_test.txt

(Note: Each number in above files means an herb or a symptom, each number is an index of the following herb list or symptom list. For example, '5' in /file/pre_herbs_train.txt means the 5th herb in the herb list /data/herbs_contains.txt, '17' in /file/pre_symptoms_train.txt means the 17th symptom in the symptom list /data/symptom_contains.txt. )

Herb list: /data/herbs_contains.txt

Symptom list: /data/symptom_contains.txt

TCM MeSH herb-symptom correspondence knowledge: /data/symptom_herb_tcm_mesh.txt

Symptom Category: /file/symptom_category.txt

# Demo

PTM(a): /src/test/RunPTMa.java (reproducing prescribing patterns discovery results)

PTM(b): /src/test/RunPTMb.java

PTM(c): /src/test/RunPTMc.java

PTM(d): /src/test/RunPTMd.java

# Herbs and symptoms prediction/recommendation tasks 
(reproducing herbs/symptoms predictive perplexity and precision@N results)

PTM(a): /src/test/PTMaPredict.java

PTM(b): /src/test/PTMbPredict.java

PTM(c): /src/test/PTMcPredict.java

PTM(d): /src/test/PTMdPredict.java

# Topic herb precision

/src/test/TopicPrecisionSymToHerb.java

# Prescription predictive perplexity

PTM(a): src/perplexity/PTMaPerplexity.java

PTM(b): src/perplexity/PTMbPerplexity.java

PTM(c): src/perplexity/PTMcPerplexity.java

PTM(d): src/perplexity/PTMdPerplexity.java
 
# Topic symptom coherence

/src/test/TopicKnowCoherence.java

