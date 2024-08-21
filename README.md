# End-2-End-Question-Answering-with-Transformers

This project includes two main parts: Retriever and Reader, with the goal of building a comprehensive system capable of extracting information from text and providing answers to questions. based on the content of the passage.
## 1. Dataset
- The dataset using in this project is SQuAD2.0 (Stanford Question Answering Dataset), which is a dataset for Question Answering task.
- Includes over 100,000 question-answer pairs on over 500 articles derived from Wikipedia articles.
- Source: https://rajpurkar.github.io/SQuAD-explorer/
## 2. Reader
- Pre-process the dataset: Prepares training and validating data for QA model by extracting questions, tokenizing and encoding text, mapping encoded positions back to the original text, and pinpointing the start and end locations of answers within the context.
- QA model: DistilBERT, Transformers (Extractive approach); LSTM (Classification approach).
- Perform train test split for training.
## 3. Evaluation
- YOLOv8: 0.956 mAP50 on validation set.
- Plain CRNN: 3.85 Val Loss, 3.87 Test loss.
- CRNN + Skip Connection: 3.1 Val loss, 3.40 Test loss.
- CRNN + Resnet: 1.63 Val loss, 1.44 Test loss.

## 4. References
- 7th International Conference on Document Analysis and Recognition (ICDAR 2003), 2-Volume Set, 3-6 August 2003, Edinburgh, Scotland, UK. IEEE Computer Society 2003, ISBN 0-7695-1960-1
