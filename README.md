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
(Provide a summary of the findings, highlighting the effectiveness of different empathy analysis methods and the results of the grammar check.)

## Contributing
Contributions to further enhance the analysis are welcome. Follow standard GitHub procedures to fork, clone, and pull request.
