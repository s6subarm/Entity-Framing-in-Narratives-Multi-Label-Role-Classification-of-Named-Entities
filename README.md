# Entity-Framing-in-Narratives-Multi-Label-Role-Classification-of-Named-Entities
This code base is a part of a larger project titled "Entity Framing in Narratives: Multi-Label Role Classification of Named Entities". This project is conducted as a part of the course work for "Introduction to Natural Language Processing" at the University of Bonn during Winter24/25 semester. This problem is a part of [SemEval 2025 Task 10](https://propaganda.math.unipd.it/semeval2025task10/).


######################################################################################################################

### Project: Entity Framing in Narratives: Multi-Label Role Classification of Named Entities


### Problem Overview
Given a news article and a named entity, the task is to classify the entity into one of three main roles: protagonist, antagonist, or innocent. Additionally, each main role has associated fine-grained roles that must also be predicted. This makes the task a multi-class, multi-label classification problem. Most existing approaches address either multi-class or multi-label problems separately, but few tackle both simultaneously. This motivated us to explore different models to see how they perform when solving both tasks together.


**********************************************************************************************************************

Approach: Fine-Tuning the Model Llama-3.2-3B-Instruct Using Pre-Constructed Prompts

**********************************************************************************************************************

### Data 
SemEval 2025 Task 10 provided a comprehensive set of [Data](https://propaganda.math.unipd.it/semeval2025task10/data/target_4_December_release.zip). For the purpose of this project only EN (English) and PT (Portuguese) are used. Partition includes train set (70%), validation set (15%) & test set (15%). Processed data is already available in [directory](Llama_3B_Instruct_with_Pre-constructed_Prompts/Dataset_EN_PT).

Annotation Heads:
    - train.csv/val.csv = [ article_id, entity_mention, start_offset, end_offset, main_role, fine_grained_roles ]
    - test.csv = [ article_id, entity_mention, start_offset, end_offset ]
Raw Texts:
    - raw-documents_EN_PT (holds the combined raw text files for both EN and PT)

Main Role Distribution:
![Data Distribution Plot](Misc/mainrole_distribution.png)

Sub Role Distribution:
![Data Distribution Plot](Misc/subrole_distribution.png)


######################################################################################################################

