######################################################################################################################

Project: Entity Framing in Narratives: Multi-Label Role Classification of Named Entities


**********************************************************************************************************************
Approach: Fine-Tuning the Model Llama-3.2-3B-Instruct Using Pre-Constructed Prompts

**********************************************************************************************************************

File Structure:
---------------
Folder: 
Llama_3B_Instruct_with_Pre-constructed_Prompts 
		
		Sub-folders:
		----->	1. code 		- holds actual codes.
		----->	2. Dataset_EN_PT 	- holds data
		----->	3. log_dir		- log directory for tensor board logs 	
		----->	4. model_cache		- cache files for model Llama 3.2 (3B) Instruct
		----->	5. tuned_model		- model checkpoints, tokenizers and logs
		----->  6. readme.txt		- current file!

**********************************************************************************************************************

Instructions:
-------------

- Please upload the Folder "Llama_3B_Instruct_with_Pre-constructed_Prompts" to Google-Drive.
- Base file path directory: "/content/drive/MyDrive/Llama_3B_Instruct_with_Pre-constructed_Prompts".

**********************************************************************************************************************


Where to start: 
---------------
1. Code -> NLP_Project_Llama_3B_instruct.ipynb

**********************************************************************************************************************

Important Notes:
—---------------
- Colab pro offers A100 (40 GB GPU RAM) and T4 (15 GB GPU RAM) run times. 
- The training was done on Google Colab Pro with A100 GPU runtime which requires around 36GB GPU RAM. 
- Tuning down the batch size can reduce it to 24GB GPU RAM.  


######################################################################################################################



