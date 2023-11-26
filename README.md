# NLP-Assignment


## Features

### Grammar Checking
- *Functionality*: A dedicated function utilizing `language_tool_python` to check and score the grammatical correctness of engineer responses.
- *Importance*: Ensures professional and error-free communication in customer service interactions.

### Empathy Analysis
Multiple methods are deployed for empathy analysis, each serving a unique purpose:

1. *TextBlob for Preliminary Sentiment Analysis*: 
   - Provides a quick and straightforward assessment of sentiment as a proxy for empathy.
   - Useful for initial screening of responses.

2. *BERT (Bidirectional Encoder Representations from Transformers)*: 
   - State-of-the-art NLP model for deeper contextual analysis.
   - More accurate in understanding the nuances of language and empathy.

3. *Logistic Regression and Random Forest Classifiers*:
   - Traditional machine learning models used to classify the level of empathy based on features extracted from text.
   - Beneficial for comparative analysis and understanding feature importance.
   - We are manually creating labeled data by using a function that is designed to assess the empathetic nature of an            engineer's response by analyzing the sentiment of the given text. The sentiment score, ranging from -1 (negative) to 1       (positive), is transformed into  an empathy label on a scale from 0 to 10, where 0 represents the least empathetic and       10 the most empathetic, for utilizing in this model.

4. *Cosine Similarity for Text Relevance*:
   - Measures how closely an engineer's response is related to the customer's query.
   - Important for ensuring that responses are not only empathetic but also contextually relevant.

### Most Efficient Method for Empathy Analysis
- *BERT stands out as the most efficient method* in this scenario due to:
   - Its ability to understand context and nuances in language better than traditional models.
   - Higher accuracy and sophistication in classifying text based on empathy.

## Usage
Execute the Jupyter Notebook to perform grammar checking and empathy analysis. The notebook includes detailed steps from data preprocessing to model evaluation.

## Data
The project uses a dataset of paired customer queries and engineer responses. Each interaction is analyzed for both grammar and empathy.

## Results

**Using an RNN (Recurrent Neural Network) or a transformer model for empathy detection in customer service interactions can indeed be a powerful approach, especially if you have enough data to support the training process

**Transformer models are resource-intensive and require significant computational power for training. They also perform best when fine-tuned on large datasets.

**Empathy Scoring Using TextBlob are determined based on sentiment polarity so indicative of only wheter a response is positive or negative.

**Text Similarity Analysis computes the cosine similarity between customer queries and engineer responses to assess the relevance of responses to the queries hence not relevant for empathy scoring.

**Training and Testing Machine Learning Models includes code for training and evaluating machine learning models (Logistic Regression, Random Forest) on the empathy scoring task.
Hyperparameter Tuning for Random Forest Model conducts grid search hyperparameter tuning for the Random Forest classifier to optimize its performance for the empathy prediction task which is most relevant for this small dataset.This can serve as a baseline and provide immediate insights.

Hence we choose Random Forest Model for final results.
Result set having ticket id as column for reference and its respective SCORE, STATUS and COMMENT for each parameter GRAMMER and EMPATHY. Result set also saved as csv in directory.


## Contributing
Contributions to further enhance the analysis are welcome. Follow standard GitHub procedures to fork, clone, and pull request.
