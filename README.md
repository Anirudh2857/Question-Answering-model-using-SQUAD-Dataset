This is a project that aims to build a question answering model using the SQuAD (Stanford Question Answering Dataset) dataset. The model will be able to answer questions based on a given passage of text, similar to how humans comprehend text and answer questions.

**Dataset**

The SQuAD dataset contains a set of Wikipedia articles with corresponding question-answer pairs. The dataset is split into two sets: train-v1.1.json and dev-v1.1.json. The former is used for training the model, while the latter is used for evaluating the model's performance.

**Model Architecture**

The model architecture used in this project is a variant of the BERT (Bidirectional Encoder Representations from Transformers) model. BERT is a pre-trained language model that has shown impressive performance in various NLP tasks, including question answering.

The BERT model is first fine-tuned on the SQuAD dataset using the train-v1.1.json file. Once the model is trained, it is evaluated on the dev-v1.1.json file. The model's performance is measured using the F1 score and exact match score.

**Conclusion**

In this project, we built a question answering model using the SQuAD dataset and a variant of the BERT model. The model is able to answer questions based on a given passage of text and has achieved a high F1 score and exact match score on the evaluation set.
