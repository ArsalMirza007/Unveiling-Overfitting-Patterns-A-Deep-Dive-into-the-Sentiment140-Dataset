# Unveiling-Overfitting-Patterns-A-Deep-Dive-into-the-Sentiment140-Dataset

# Instructions:
Tasks performed in the provided code:

1. **Exploring Overfitting in NLP**: The code begins with an introduction to the assignment, explaining that the objective is to create a model architecture that does not overfit using techniques learned in previous weeks.

2. **Defining Useful Global Variables**: Global variables such as EMBEDDING_DIM, MAXLEN, TRUNCATING, PADDING, OOV_TOKEN, MAX_EXAMPLES, and TRAINING_SPLIT are defined. These variables are essential for data preprocessing and model training.

3. **Explore the Dataset**: The code provides insights into the Sentiment140 dataset by displaying the structure of the dataset and showcasing examples of the data points.

4. **Parsing the Raw Data**: A function called `parse_data_from_file` is defined to extract sentences and labels from the CSV file containing the dataset. The labels are converted to integers where 0 represents negative sentiment and 1 represents positive sentiment.

5. **Random Sampling**: Only 10% of the original dataset is sampled randomly to reduce execution time while maintaining diversity in the data.

6. **Training-Validation Split**: The dataset is split into training and validation sets using the `train_val_split` function. This ensures that the model can be trained on one set and validated on another to assess its performance.

7. **Tokenization - Sequences, Truncating, and Padding**: The text data is tokenized, sequences are generated, and padding/truncating is performed to ensure uniform length sequences, which are essential for training the model.

8. **Using Pre-defined Embeddings**: Pre-trained word embeddings from GloVe are used to represent words in the vocabulary, enhancing the model's performance.

9. **Define a Model That Does Not Overfit**: A neural network model architecture is defined using Keras. The model includes layers such as Embedding, GlobalMaxPooling1D, Dense, and Dropout to prevent overfitting and achieve effective sentiment classification.

10. **Model Training**: The defined model is trained on the training data, and the training history is stored for evaluation.

11. **Evaluation**: The model's performance is evaluated by plotting the training and validation loss curves. Criteria for passing the assignment are provided based on the slope of the validation loss curve.

12. **Saving Training History**: The training history is saved in a pickle file for further analysis or comparison.

Overall, the code provides a comprehensive workflow for exploring, preprocessing, training, and evaluating a neural network model for sentiment analysis while addressing the challenge of overfitting.

# The Dataset will be fetched online by the Kaggle Link

![loss](https://github.com/ArsalMirza007/Unveiling-Overfitting-Patterns-A-Deep-Dive-into-the-Sentiment140-Dataset/assets/121928372/fd2e0aba-3e10-42d1-ad9c-36f0a621256c)
![accuracy](https://github.com/ArsalMirza007/Unveiling-Overfitting-Patterns-A-Deep-Dive-into-the-Sentiment140-Dataset/assets/121928372/0c682107-ce9c-4612-b50e-cd8ceeaa51bb)

