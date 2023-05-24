# ❄️ medical_knowledge_graph
this is a knowledge graph with diseases and symptoms as the main entities

#### 💡 What are knowledge graphs? 

here is link of blog written by us that describes what knowledge graphs are and how to make them 
https://medium.com/everythingisconnected

made during our internship under JIO this projects aims to build a knowledge graph of medical domain 

### 📚 about the dataset

* There are 2 datasets one with the diseases (in UMLS code) and symptoms (UMLS) 
* and other with diseases (in MESH code) and Medicines used to cure them (MESH)
* need to find a way to convert the MESH code to UMLS code so a third medicine identity can be added to the database

#### 📕 kg_data dataset:-

* this csv contains all the info of the diseases and their symptoms and the number of occurance of the disease.
* this dataset has 1863 rows
* 134 unique diseases and  401 unique symptoms
* the diseases are presented in UMLS code
* source of the dataset https://people.dbmi.columbia.edu/~friedma/Projects/DiseaseSymptomKB/index.html

| #   | Column     | Dtype   |
|:---: | :------: |  :-----: |
| 0   | Disease   |  object / string   |
| 1   | Count of Disease Occurrence     |  object / string  |
| 2   | Symptom       |  object / string   |

![image](https://github.com/aryanrathore1012/medical_knowledge_graph/assets/91218998/b5eb1298-2692-4b4d-bd89-18f4a67a6a9e)

#### 📗 DCh-Miner_miner-disease-chemical.tsv:-

* this csv contains the diseases in mesh code and the medicine used to cure the disease both are in MESH code just google the mesh code and you will find the corresponding entity

* have to find a way to convert the diseases in this csv to UMLS to add medicines to the medical_knowledge_graph

* source: https://snap.stanford.edu/biodata/datasets/10004/10004-DCh-Miner.html 

| #   | Column    | Non-Null Count  | Dtype    | 
| :---:  | :------: | :--------------: | :-----: | 
| 0   | # Disease(MESH)   | 15000 non-null  | int64    |
| 1   | Chemical  | 15000 non-null  | float64  |

![image](https://github.com/aryanrathore1012/medical_knowledge_graph/assets/91218998/e7349b93-e438-4669-b583-2c09245667e6)


# 🖋️ insights

#### 1. the jsons are a result of running the drug_check.ipynb data in these jsons has been uploaded to the arangodb database.

#### 🖋️ 2 IMP. it is highly reccomond you run the ipynb once for yourself to get appropriate key_ for diseases and symptoms 

# Result:-  

* a photo of medical_knowledge_graph 
* NOTE this is a small samples of values actually present in the database
* the acutal graph has way more values the shown in this output
* here the grey dots are the diseases and purple the symptoms
* the green lines are the connection between these dots representing which Symptom is related to what disease

![WhatsApp Image 2023-05-22 at 12 17 48](https://github.com/aryanrathore1012/medical_knowledge_graph/assets/91218998/7e5cdf6a-5361-40b2-9da3-4c66b1aa562a)

# 🔜 future ugrades

* need to find out a way to convert the disease from MESH code to UMLS code so a whole new medicine entity could be joined to the graph

# 👨‍🦱credits and contact info:-

* made by Aryan Rathore
* LinkedIn : https://www.linkedin.com/in/aryan-rathore-b15459215/
* email: aryanrathore13572002@gmail.com, aryan.rathore2021@vitbhopal.ac.in
* and Reva Bharara
* email: bhararareva@gmail.com, revabharara@gmail.com
* LinkedIn : https://www.linkedin.com/in/reva-bharara-a83a78241/


# ---------------------------------------
