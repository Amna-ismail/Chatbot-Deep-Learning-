# Chatbot-Deep-Learning-
The goal of this project was to create a deep learning-based chatbot capable of handling basic conversational queries. The chatbot was trained using a small dataset with predefined questions and responses.

Data Preparation
1.	Dataset: A simple JSON dataset was created with intents, patterns (user inputs), and responses (bot outputs).
2.	Loading the Data: The JSON file was loaded, and patterns and responses were extracted.
3.	Tokenization: Patterns were tokenized using Keras' Tokenizer.
4.	Sequencing and Padding: Tokenized patterns were converted to sequences and padded to ensure uniform input length.
5.	Label Encoding: Intents were encoded as integers and one-hot encoded for training.

Model Architecture
An LSTM-based neural network was built using Keras. The model architecture is as follows:
1.	Embedding Layer: Converts word indices to dense vectors of fixed size.
2.	LSTM Layer: 128 units, returns sequences for stacking LSTMs.
3.	Dropout Layer: 0.5 dropout rate to prevent overfitting.
4.	LSTM Layer: 128 units.
5.	Dropout Layer: 0.5 dropout rate.
6.	Dense Layer: 128 units, ReLU activation.
7.	Dense Layer: Number of intents, softmax activation.

Model Training
Model Deployment

Conclusion
The project successfully demonstrated the creation and deployment of a deep learning-based chatbot. While the chatbot handled basic queries effectively, further improvements could be made by using a larger and more diverse dataset, enhancing the model architecture, or incorporating advanced NLP techniques like attention mechanisms.
