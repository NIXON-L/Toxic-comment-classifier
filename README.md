# Toxic-comment-classifier
In the age of online communication, the prevalence of toxic comments poses a significant challenge to maintaining healthy discourse and fostering a safe environment. The rise of online platforms has revolutionized communication, yet it has also brought to light a concerning issue: the proliferation of toxic comments. This project addresses the imperative need for automated tools to identify and categorize toxic behaviours within text data. Leveraging a large dataset of Wikipedia comments annotated with labels for various types of toxicity including toxic, severe toxic, obscene, threat, insult, and identity hate, a deep learning model utilizing Long Short-Term Memory (LSTM) architecture is proposed. The LSTM-based model offers a robust framework for sequential data processing, making it well-suited for the nuanced task of toxic comment classification.

**#The specific goals of the project include:**


1.	Gather a large dataset of annotated comments from online platforms, preprocess the textual data to remove noise and irrelevant information, and prepare it for model training and evaluation.
2.	Design and implement an LSTM-based deep learning architecture for toxic comment classification, leveraging the sequential nature of textual data to capture long-range dependencies and contextual information.
3.	Train the Toxic Comments Classifier using the annotated dataset, fine-tuning model hyperparameters, optimizing training algorithms, and incorporating techniques to address class imbalances and overfitting.
4.	Evaluate the performance of the classifier using standard metrics such as binary accuracy and conduct comprehensive analyses to assess its effectiveness in detecting and categorizing toxic comments across different types of toxicity.
5.	My future work aims to integrate the trained classifier into online platforms or moderation tools, enabling real-time detection and moderation of toxic comments, and assess its usability, scalability, and impact on user experience and community dynamics.
6.	By achieving these objectives and goals, this project aims to contribute to the development of automated tools and technologies for combating toxic behaviour in online discourse, promoting a safer, healthier, and more inclusive digital environment for users worldwide.


** #labels in the datasets:**

 1. Toxic Comments:
The dataset comprises 144,277 non-toxic comments (labelled as 0) and 15,294 toxic comments (labelled as 1). Insight: Toxic comments represent a significant portion of the dataset, indicating a notable presence of negative or harmful discourse.

2.Severe Toxic Comments:
Among the comments, 157,976 are labelled as non-severe toxic (0), while 1,595 comments exhibit severe toxicity (1). Insight: Although severe toxic comments constitute a smaller proportion of the dataset, their presence highlights instances of extreme toxicity that necessitate attention.

3.Obscene Comments:
Majority of the comments (151,122) are labelled as non-obscene (0), while 8,449 comments are classified as obscene (1). Insight: Obscene comments, although less prevalent compared to non-obscene comments, still represent a considerable portion of the dataset, indicating instances of offensive or inappropriate content.

4.Identity Hate Comments:
Most comments (158,166) do not exhibit identity hate (labelled as 0), while 1,405 comments demonstrate identity-based hate speech (labelled as 1). While identity hate comments constitute a smaller fraction of the dataset, their presence underscores the prevalence of discriminatory behaviour within online discourse.

5.Insulting Comments:
A majority of comments (151,694) are devoid of insults (labelled as 0), while 7,877 comments contain insults (labelled as 1). Insight: Insulting comments, though less frequent compared to non-insulting comments, still manifest instances of verbal abuse or personal attacks, reflecting negative interactions within the dataset.
![SUMMARY](https://github.com/user-attachments/assets/0715d5a9-a49b-4dbf-a50d-8dae138f2761)

**#About deep learning model used:**
A Bidirectional LSTM layer is then incorporated to capture contextual information from both past and future states of the sequence. Subsequent dense layers with ReLU activation functions increase the model's capacity to learn complex patterns in the data. Finally, a dense layer with a sigmoid activation function is used for multi-label classification, predicting the probability of each class independently. After defining the model architecture, it is compiled using the Adam optimizer and binary cross-entropy loss function, which are suitable for binary classification problems. Additionally, binary accuracy is chosen as the evaluation metric to monitor the model's performance during training. Model building involves designing and training a machine learning or deep learning model to perform a specific task, such as toxicity classification. In my project, I constructed a deep learning model using TensorFlow's Sequential API. The model architecture includes layers for text vectorization, word embedding, LSTM, and dense layers for classification. During model building, I defined the architecture, compiled the model with appropriate loss and optimization functions, and trained it on the training dataset using backpropagation. After training, the model learns to make predictions based on the input text's features and the toxicity labels.
