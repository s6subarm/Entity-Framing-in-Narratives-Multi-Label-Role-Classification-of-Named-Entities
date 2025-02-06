# Entity-Framing-in-Narratives-Multi-Label-Role-Classification-of-Named-Entities
This code base is a part of a larger project titled "Entity Framing in Narratives: Multi-Label Role Classification of Named Entities". This project is conducted as a part of the course work for "Introduction to Natural Language Processing" at the University of Bonn during Winter24/25 semester.


###########################################################################################

### Project: Entity Framing in Narratives: Multi-Label Role Classification of Named Entities


### Problem Overview
Given a news article and a named entity, the task is to classify the entity into one of three main roles: protagonist, antagonist, or innocent. Additionally, each main role has associated fine-grained roles that must also be predicted. This makes the task a multi-class, multi-label classification problem. Most existing approaches address either multi-class or multi-label problems separately, but few tackle both simultaneously. This motivated us to explore different models to see how they perform when solving both tasks together.


************************************************************************************
Approach: Fine-Tuning the Model Llama-3.2-3B-Instruct Using Pre-Constructed Prompts

************************************************************************************

Structure of the files:
-----------------------
1. code 		- holds actual codes.
2. Dataset_EN_PT 	- holds data
3. log_dir		- log directory for tensor board logs 	
4. model_cache		- cache files for model Llama 3.2 (3B) Instruct
5. others		- misc. Includes poster, problem formulation, etc.
6. tuned_model		- model checkpoints, tokenizers and logs

************************************************************************************

Where to start: 
---------------
1. Code -> NLP_Project_Llama_3B_instruct.ipynb

************************************************************************************

Important Notes:
—---------------
- Colab pro offers A100 (40 GB GPU RAM) and T4 (15 GB GPU RAM) run times. 
- The trained was done on Google Colab Pro with A100 GPU runtime. With the current set of parameters, it requires around 36GB GPU RAM. 
- Tuning down the batch size can reduce it to 24GB GPU RAM.

###########################################################################################

