

1. Data for the models can be downloaded from 
Data can be downloaded from : https://www.kaggle.com/datasets/parthplc/facebook-hateful-meme-dataset

2. Description of files in the folder
---> Standard Models Final.ipynb : Standard ML model performance using text only tf-idf vectors
---> BERT-final.ipynb: BERT based unimodal classifier
---> Visual Bert Final.ipynb: Visual BERT based multimodal approach
---> CLIP-Final.ipynb: MMBT + CLIP based multimodal approach
---> Deepface Final.ipynb: Deepface for facial feature extraction
---> Google_WebDetection-Final.ipynb: Google web entity detection model. This requires service account file to access cloud vision API. The same has been included as myproject-svyerra-40d2858a7beb.json

3. Final datafiles
---> output_entities.csv: output entities extracted 
---> final_cleaned_with_all_tags.csv: final augmented file with original + features from Google Web detection model and Deepface
---> new_merged.csv: Merged data for standard ML models
