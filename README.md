# **Entity Framing in Narratives: Multi-Label Role Classification of Named Entities**

This codebase is part of the project **"Entity Framing in Narratives: Multi-Label Role Classification of Named Entities"**, conducted for the **"Introduction to Natural Language Processing"** course at the **University of Bonn** during the **Winter 24/25 semester**.  
The problem is a part of **[SemEval 2025 Task 10](https://propaganda.math.unipd.it/semeval2025task10/)**.

---

## **Project Overview**
The goal is to classify named entities in news articles into one of three main roles:  
- **Protagonist**
- **Antagonist**
- **Innocent**

Additionally, each main role has associated **fine-grained roles** that need to be predicted, making this a **multi-class, multi-label classification problem**.  
Most existing approaches address either multi-class or multi-label tasks separately, but this project explores models that tackle both tasks simultaneously.

---

## **Approach**
- Fine-tuning **LLaMA-3.2-3B-Instruct** using **pre-constructed prompts** for multi-label classification.

---

## **Data Description**
The dataset is provided by **[SemEval 2025 Task 10](https://propaganda.math.unipd.it/semeval2025task10/data/target_4_December_release.zip)**.  
This project uses **English (EN)** and **Portuguese (PT)** data, partitioned as follows:
- **Training Set:** 70%
- **Validation Set:** 15%
- **Test Set:** 15%

Processed data is stored in the **[Dataset_EN_PT directory](Llama_3B_Instruct_with_Pre-constructed_Prompts/Dataset_EN_PT)**.

---

### **Annotation Format**
- **Train/Validation Files:**  
  `train.csv`, `val.csv` – [article_id, entity_mention, start_offset, end_offset, main_role, fine_grained_roles]
- **Test File:**  
  `test.csv` – [article_id, entity_mention, start_offset, end_offset]

### **Raw Texts**  
The **raw-documents_EN_PT** directory holds the combined raw text files for both English and Portuguese.

---

## **Data Distribution**

### **Main Role Distribution**
![Main Role Distribution](Misc/mainrole_distribution.png)

### **Sub Role Distribution**
![Sub Role Distribution](Misc/subrole_distribution.png)

---

