# Hateful Meme Identification Using Multi-Modal Approach

## Introduction
This project aims to identify hateful memes by combining different modalities, such as text and images, to understand and detect multimodal hate speech. Hateful memes present a unique challenge as they often combine seemingly innocuous images and text to convey hateful messages.

## Dataset
The dataset, created by FacebookAI, consists of 10,000 images in JSONL format, including 'train.jsonl' (8500 samples) and 'dev_seen.jsonl' (1040 samples). Each data point includes an ID, image path, text, and a label indicating whether the meme is hateful or not.

## Methods
### Unimodal Approaches
- Text feature extraction using TF-IDF.
- Classification models: Logistic Regression, Naive Bayes, Random Forest, SVM, KNN.
![Unimodal1](img/unimodal1.png)

- BERT-based model using bert-base-uncased from Transformer Library.
![Unimodal2](img/unimodal2.png)

### Multi-modal Approaches
- Visual BERT: A multi-modal vision and language model trained using COCO.
![Visual Bert](img/Visual_bert.png)

- MMBT + CLIP (OpenAI): Uses text features from BERT and ResNet for image encoding, flexible for feature embeddings.
![MMBT CLIP](img/mmbt-clip.png)

### Feature Augmentation
- Facebook Deep Face algorithm: Extracts features from images for age, emotion, gender, and race classification.
![Deepface](img/deepface.png)
- Google Web Detection Model: Detects web entities and provides context for images.
![Google Web Detection](img/Google_web_detection.png)

## Results
- Improvement in accuracy and AUC scores with multi-modal approaches compared to unimodal ones.
![Results](img/Results.png)
- The best performance achieved with the MMBT + CLIP approach.
![MMBT_CLIP](img/mmbt_clip_results.png)

## Future Work
- Exploring better feature processing methods.
- Dataset augmentation with manually labeled features.
- Ensembling methods like Vil-BERT, UNITER, Ernie-Vil on augmented features.

## References

- [Visual Bert](https://arxiv.org/abs/1908.03557)
- [CLIP](https://openai.com/research/clip) 
- [Facebook Meme Competition](https://ai.meta.com/blog/hateful-memes-challenge-and-data-set/)
- [Dataset Augmentation Approach](https://github.com/dsfsi/textaugment#eda-easy-data-augmentation-techniques-for-boosting-performance-on-text-classification-tasks)
- [CLIP + MMBT approach](https://towardsdatascience.com/how-to-get-high-score-using-mmbt-and-clip-in-hateful-memes-competition-90bfa65cb117)
- [Facebook Deep Face](https://research.facebook.com/publications/deepface-closing-the-gap-to-human-level-performance-in-face-verification/)
- [Google Web Detection Model](https://cloud.google.com/vision/docs/detecting-web)
