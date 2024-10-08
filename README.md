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

### Setup Instructions

Create a virtual environment and install the required packages. Once your environment is ready, start Jupyter Notebook to begin working on the exercises.

---

## Iteration 1: Tokenization and Text Preprocessing

- Import the necessary libraries from the Hugging Face `transformers` library.
- Choose a pre-trained tokenizer (such as BERT or GPT) and tokenize a given sentence.
- Explore the tokenization process by converting the tokens back into words.

---

## Iteration 2: Understanding Embeddings

- Define a function to extract embeddings from a pre-trained model.
- Visualize the embeddings using techniques like PCA or t-SNE to see how similar words are clustered.

---

## Iteration 3: Text Classification Task

- Load a pre-trained text classification model from Hugging Face.
- Preprocess a dataset and perform classification using the model.
- Evaluate the model’s performance using metrics such as accuracy and F1-score.

---

## Iteration 4: Text Summarization Task

- Use a pre-trained summarization model from Hugging Face (e.g., BART or T5).
- Summarize a sample article and evaluate the quality of the summary.
- Experiment with different prompts to generate summaries of varying lengths and focus.

---

## Iteration 5: Comparison of Pre-trained LLMs

- Compare the output of different LLMs (such as GPT-2 and BERT) on the same text classification or summarization tasks.
- Analyze the differences in performance, generation style, and accuracy of the models.

---

## Iteration 6: Cross-Validation of Text Generation

- Generate text from different models and observe the variations in coherence and fluency.
- Visualize the attention mechanisms of a transformer model during the text generation process.

---

## Bonus: Fine-Tuning a Pre-trained Model

- Fine-tune a pre-trained LLM on a custom dataset.
- Use this fine-tuned model for text classification or summarization, and compare the results to the original pre-trained model.

---

## Submission

Once you have completed the lab, push your Jupyter notebook to your forked GitHub repository and create a pull request.

```bash
$ git add .
$ git commit -m "completed lab"
$ git push origin main
```
