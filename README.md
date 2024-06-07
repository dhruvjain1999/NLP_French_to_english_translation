## Contributors
- Dhruv Jain: Feature engineering, model development, summary, future work.
- Sunday Okechukwu: Data gathering, data cleaning, data pre-processing, evaluation, results.

## Machine Translation
### What is Machine Translation?
Machine Translation refers to the automated process of translating text or speech from one language (source language) to another language (target language). For example, translating from French to English or Spanish to English.

### Why Machine Translation?
- **Internal Communication**: Helps companies with operations in multiple countries manage communication across languages.
- **Data Analysis**: Enables analysis of large amounts of content from social media and websites in different languages for insights.
- **Online Customer Service**: Supports customer service by translating requests and responses accurately.
- **Legal Research**: Aids in preparing legal documents in different languages.

### Common Types of MT
- Rule-based MT
- Statistical MT
- Neural MT

## Project Goal
The goal of this project is to build a deep neural network for Neural Machine Translation, accepting French sentences as input and returning English translations.

## Dataset
- Dataset: [Available here](dataset_link)
- French-English dataset with 217,975 sentences

## Main Stages of the Project
1. **Preprocessing**: Normalizing case, removing punctuation and non-alphabetic characters, tokenization, and padding.
2. **Feature Extraction**: Training word embeddings using Keras embedding layer.
3. **Modeling**: Seq2Seq model with LSTM layers for both encoder and decoder.
4. **Evaluations**: BLEU score for translation quality.
5. **Summary and Future Work**: Suggestions for improvement like increasing LSTM layers, using pre-trained embeddings, and implementing attention mechanism.

### Preprocessing
- Normalize case to lowercase and Unicode normalization.
- Remove punctuation and non-alphabetic characters.
- Tokenize words into IDs and add padding for fixed-length sequences.

### Feature Extraction
- Train word embeddings using the Keras embedding layer.
- Convert words into fixed-length vectors.

### Model Development
- Use a Seq2Seq model with LSTM layers for both encoder and decoder.
- Encoder processes input sequence into a context vector.
- Decoder predicts target sequence based on the context vector.

### Evaluations and Results
- Train Set Results: [Results](train_results)
- Test Set Results: [Results](test_results)
- BLEU-4 Score: 0.849

### Summary and Future Works
- Improve the model by increasing the number of LSTM layers.
- Use pre-trained embedding layers like word2vec or GloVe.
- Implement attention mechanism for better performance.
