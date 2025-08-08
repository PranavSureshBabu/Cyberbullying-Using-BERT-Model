# Cyberbullying-Using-BERT 

Link to the Project -https://nbviewer.org/github/PranavSureshBabu/Cyberbullying-Using-BERT-Model/blob/main/Cyberbullying_Classification_using_BERT.ipynb

## OVERVIEW

This solution applies Natural Language Processing (NLP) techniques using BERT (Bidirectional Encoder Representations from Transformers) to detect and classify cyberbullying content from social media text. It aims to identify toxic behavior online, ensuring safer digital spaces, especially for vulnerable users.

<img width="940" height="626" alt="image" src="https://github.com/user-attachments/assets/30115650-8fa0-4079-aa3d-6e0555e27a42" />

 
## Goal / Objective

The main objective is to build an intelligent system that can:

- Automatically detect cyberbullying in text.

- Categorize abusive content into types like hate speech, sexual harassment, and threats.

- Assist moderation teams in flagging harmful content early, improving response time and platform safety.

## IMPLEMENTATION

1. Understanding the Problem

Cyberbullying is a growing concern across online platforms. Manual moderation is slow and subjective. Automating this process using deep learning helps maintain real-time safety and consistency in decision-making.

2. Data Collection & Preprocessing

The dataset contains social media posts labeled into various types of cyberbullying. Preprocessing involved:

 - Cleaning and lowercasing text

 - Removing special characters, stopwords, and URLs

 - Tokenizing and encoding text using BERT’s tokenizer

3. Modeling with BERT

We used the pre-trained BERT base model and fine-tuned it for text classification. BERT’s architecture helps the model understand context and relationships between words — making it far superior to traditional models in detecting subtle abusive language.

4. Training

 - Trained on labeled posts using a custom classification head on top of BERT.

 - Used attention masks to preserve sentence structure.

 - Loss and accuracy were monitored across training and validation sets.

5. Evaluation

- Evaluated the model using accuracy, F1-score, and confusion matrix.

- Real-world abusive content samples were tested to verify performance.


## WHY BERT?

- It understands context better than traditional models — crucial in identifying subtle or sarcastic bullying.

- It is pre-trained on large-scale data, so it adapts well to specific tasks like abuse detection with minimal fine-tuning.

- Its bidirectional nature allows it to look at both the left and right context of a word, helping detect hidden or nuanced abusive intent.

## Tools & Technologies Used

- Python

- Pandas / NumPy for data manipulation

- PyTorch for model training

- Transformers (HuggingFace) for BERT model and tokenizer

- Matplotlib / Seaborn for data visualization

## RESULTS

- Achieved 93–95% accuracy on the test set, showing strong generalization across multiple types of abuse.

- The model was able to correctly flag abusive content with high precision, reducing false positives that could lead to unfair content removal.

- Helpful for social media platforms, forums, and educational institutions aiming to monitor and manage toxic behavior at scale.


## CHALLENGES FACED

- Working with long and noisy text data — preprocessing was essential to clean slang, emojis, and inconsistent formatting in social media content.

- Fine-tuning BERT effectively — required careful hyperparameter tuning to avoid overfitting while still capturing the complex patterns in abusive language.
  
