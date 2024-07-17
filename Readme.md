AgroBot - A Telugu Agricultural Chatbot


AgroBot is a professional chatbot developed specifically to cater to the needs of Telugu-speaking farmers in India. The methodology adopted for developing the chatbot involved a systematic process that encompassed data collection, data preprocessing, feature extraction and representation, model development, model training and evaluation, user interaction, and iterative improvement. AgroBot incorporates advanced technologies, including speech-to-text and text-to-speech functionality, along with a graphical user interface (GUI) for ease of use.

Features:

Dataset: AgroBot was developed using a dataset of 1,500 agricultural questions and corresponding answers in Telugu. The dataset was collected from reliable sources such as agricultural forums, government websites, and domain experts, ensuring relevance, accuracy, and diversity in the types of agricultural queries.

Speech-to-Text Functionality: AgroBot allows users to interact through voice commands or query or audio files. The chatbot system employs various techniques, including audio preprocessing to reduce background noise, conversion of audio to text using the Google Speech-to-Text API, and integration of the converted text as input for the chatbot.

Data Preprocessing: The collected dataset underwent preprocessing steps, including cleaning and normalization of text. Punctuation, special characters, and irrelevant or duplicate entries were removed. Tokenization techniques were applied to split the text into individual words or tokens.

Feature Extraction and Representation: The preprocessed text data was transformed into numerical representations using the Tfidf Vectorizer from the scikit-learn library.This vectorization technique assigned weights to words based on their frequency in specific questions and across the entire dataset, capturing the importance of words in differentiating between various agricultural queries.

Cosine Similarity for Question Matching: AgroBot utilizes cosine similarity to identify similar questions and provide relevant answers. The cosine similarity measure compares the similarity between user input questions and the preprocessed question vectors in the dataset, enabling the chatbot to retrieve the most similar question and its corresponding answer.

Deep Learning Model: AgroBot employs a deep learning approach using the TensorFlow and Keras libraries to build the chatbot model. The model architecture consists of an embedding layer, LSTM layer, and dense output layer. The embedding layer learns the representation of words in a continuous vector space, capturing semantic relationships, while the LSTM layer processes sequential information and captures contextual dependencies.


How to run:

Install the required dependencies listed in the requirements.txt file.(pip install -r requirements.txt)
Ensure that the dataset file, agrobot_dataset.xlsx, is placed in the appropriate directory.
Run the main script using jupyter noteboo or google colab "AgroBot_Team1.ipynb" to start the AgroBot chatbot.
Follow the prompts and enter your queries or use voice commands/audio files to interact with AgroBot.
AgroBot will process your input and provide accurate and contextually relevant responses based on the Telugu dataset and advanced technologies incorporated.
Gui can be launched from the the ipynb file itself by executing the code .

We hope AgroBot proves to be a valuable tool for Telugu-speaking farmers, enhancing their agricultural practices and productivity!