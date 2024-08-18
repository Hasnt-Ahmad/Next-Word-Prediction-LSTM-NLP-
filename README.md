# Next-Word-Prediction-LSTM-NLP

This project demonstrates a Next Word Prediction model using TensorFlow and Keras. The model is trained on a dataset of text titles, and it generates the most probable next words based on a given seed text.

**Key Features:**
 **1.Data Preprocessing:** The dataset is cleaned by removing unwanted characters and converting text to sequences.
**2.Text Tokenization:** The Tokenizer class from Keras is used for converting words to sequences, and handling out-of-vocabulary words.
**3.Model Architecture:** The model is built using a Sequential API with the following layers:
    **Embedding Layer:** Converts word indices into dense vectors of fixed size.
    **Bidirectional LSTM:** Captures information from both directions in a sequence.
    **Dense Layer:** Outputs a probability distribution over the entire vocabulary.
    **Training:** The model is trained with categorical cross-entropy loss and Adam optimizer for 50 epochs.
    **Prediction:** After training, the model predicts the next words for a given seed text, generating coherent and contextually relevant text.

**How to Use:**
    **Dataset:** Ensure the dataset (medium_data.csv) is loaded and preprocessed.
  *  *Training:** Run the training code to fit the model on the input sequences.
    **Prediction:** Input a seed text to generate the next words using the trained model.
**Dependencies:**
    **TensorFlow**
    **Pandas**
    **NumPy**
     
**Example:**
Given the seed text "implementation of", the model might predict the next words to be something like "the system" or "a process", depending on the learned patterns.
