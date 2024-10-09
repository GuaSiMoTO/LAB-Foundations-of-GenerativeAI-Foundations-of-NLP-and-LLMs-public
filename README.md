# LAB-Foundations-of-NLP-and-LLMs

## Introduction
In this lab, students will explore the basic concepts of Natural Language Processing (NLP), including tokenization, embeddings, and their application in Large Language Models (LLMs). We will focus on text preprocessing tasks and compare how different pre-trained models handle tasks such as classification, summarization, or translation. The goal is to understand the role of embeddings and transformers in handling different NLP tasks.

Students will:
1. Learn about tokenization and embeddings.
2. Explore text preprocessing methods.
3. Implement basic NLP tasks using pre-trained LLMs.
4. Compare the performance of models in different tasks.

---

## Initial Setup

### Requirements
Fork the provided GitHub repository to your account, and clone it locally. This will be your workspace for the lab exercises.

- [Learn how to fork this repo](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project)
- Clone this repo into your code/labs folder.

```bash
git clone https://github.com/codeskills-ai/LAB-Foundations-of-NLP-and-LLMs.git
cd LAB-Foundations-of-NLP-and-LLMs
```

### Setup Instructions

Create a virtual environment and install the required packages.
```bash
pip install -r requirements.txt
```

 Once your environment is ready, start Jupyter Notebook to begin working on the exercises.

 ```bash
jupyter notebook
```

---

## Iteration 1: Tokenization and Text Preprocessing

- Import the BERT tokenizer: Use the pre-trained BERT tokenizer from the Hugging Face transformers library.
- Tokenize a sentence: Input the following sample sentence: "Natural language processing is transforming the way computers understand human language."
- Convert tokens back to words: After tokenizing the sentence, convert the tokens back to human-readable text to understand how BERT processes the input.

---

## Iteration 2: Understanding Embeddings

- Load BERT model: Use the pre-trained BERT model (bert-base-uncased) from Hugging Face.
- Extract embeddings: Pass the same sample sentence from Iteration 1 through BERT and extract the token embeddings.
- Visualize embeddings: Apply dimensionality reduction (e.g., PCA or t-SNE) to visualize the token embeddings in 2D space. Identify how semantically similar words cluster together.

---

## Iteration 3: Text Classification Task

- Load the DistilBERT model: Use the pre-trained DistilBERT model (distilbert-base-uncased) from Hugging Face for a binary sentiment classification task (positive/negative).
- Dataset: Use the IMDb movie reviews dataset. Preprocess the dataset by tokenizing the text using the DistilBERT tokenizer.
- Perform classification: Input a review (e.g., "The movie was fantastic!") and classify it as either positive or negative.
- Evaluate performance: Use metrics like accuracy and F1-score to evaluate the model's performance on the test dataset.

---

## Iteration 4: Text Summarization Task

- Load the BART model: Use the pre-trained BART model (facebook/bart-large-cnn) from Hugging Face for text summarization.
- Input text: Use the following text from a news article or choose a lengthy paragraph from any resource: "Artificial intelligence is reshaping many industries by automating tasks, providing deep insights, and creating new ways to solve complex problems..."
- Generate a summary: Use BART to summarize the text into a few sentences.
- Experiment with length: Modify the prompt or parameters to generate a more detailed or a more concise summary.

---

## Iteration 5: Comparison of Pre-trained LLMs

- Compare the output of different LLMs (such as GPT-2 and BERT) on the same text classification or summarization tasks.
- Analyze the differences in performance, generation style, and accuracy of the models.

---

## Iteration 6: Cross-Validation of Text Generation

- Load GPT-2 and BERT: Use the pre-trained GPT-2 (gpt2) and BERT (bert-base-uncased) models from Hugging Face.
- Task: Use both models to generate text from the following prompt: "In the future, artificial intelligence will change the way humans...".
- Compare outputs: Generate text using GPT-2 and classify text using BERT (for sentiment analysis) using the same dataset as in Iteration 3.
- Evaluate text consistency: Analyze the fluency and coherence of the generated text. Are there any common issues such as repetition, nonsensical text, or logical gaps?

---

## Bonus: Fine-Tuning a Pre-trained Model

- Dataset: Use the IMDb movie reviews dataset again but fine-tune the DistilBERT model to better handle sentiment classification.

- Fine-tune DistilBERT: Fine-tune the DistilBERT model on the IMDb dataset, adjusting the learning rate and other hyperparameters to optimize performance.

- Evaluate the model: After fine-tuning, evaluate the model’s performance on a validation set. Compare the results to the original pre-trained model.

---

## Submission

Once you have completed the lab, push your Jupyter notebook to your forked GitHub repository and create a pull request.

```bash
$ git add .
$ git commit -m "completed lab"
$ git push origin main
```
