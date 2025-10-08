# **Investigative Analysis on the IMDb Sentiment Analysis Task**

This repository contains the official codebase for the research paper, "Investigative Analysis on the IMDb Sentiment Analysis Task," authored by Partha Thakuria, Nischal Parne, and Kaushik Sai Kadali.

The project validates the core findings of the paper by implementing and comparing a classic baseline model against a modern, pre-trained Transformer model (BERT) for sentiment analysis on the IMDb movie review dataset.

## **Project Overview**

The goal of this project is to demonstrate the performance gap between traditional machine learning models and modern Large Language Models (LLMs) for a standard NLP task. The script provided here will:

1. Load a sample of the IMDb dataset.  
2. Train and evaluate a **Baseline Model** using TF-IDF vectorization and a Logistic Regression classifier.  
3. Load a pre-trained **BERT model** from Hugging Face and fine-tune it on the same dataset.  
4. Evaluate the fine-tuned BERT model.  
5. Present a final comparison of the accuracies of both models.

## **Tech Stack**

* **Python 3.8+**  
* **PyTorch**: For building and training the deep learning model.  
* **Hugging Face Transformers**: To easily download and use the pre-trained BERT model.  
* **Hugging Face Datasets**: For efficiently loading the IMDb dataset.  
* **Scikit-learn**: For the baseline model and performance metrics.  
* **Pandas**: For data manipulation.

## **Setup and Installation**

1. **Clone the repository:**  
   git clone \[https://github.com/your-username/imdb-sentiment-analysis.git\](https://github.com/your-username/imdb-sentiment-analysis.git)  
   cd imdb-sentiment-analysis

2. **Create and activate a virtual environment (recommended):**  
   python \-m venv venv  
   source venv/bin/activate  \# On Windows, use \`venv\\Scripts\\activate\`

3. **Install the required dependencies:**  
   pip install \-r requirements.txt

## **How to Run**

After setting up the environment, you can run the entire analysis with a single command. The script will automatically download the necessary dataset and pre-trained models.

python analysis.py

The script uses a sample of 1000 reviews by default to ensure it runs quickly on a standard machine without a dedicated GPU. This process may still take several minutes, especially during the model downloading and fine-tuning steps.

## **Expected Results**

The output will show the performance of both models. You should expect to see a significant accuracy improvement from the fine-tuned BERT model, demonstrating the power of Transformer architectures.

\--- Final Results Comparison \---  
Baseline (TF-IDF \+ Logistic Regression) Accuracy: \[An accuracy around 0.80 \- 0.85\]  
Advanced (Fine-tuned BERT) Accuracy: \[An accuracy above 0.90\]

Conclusion: The fine-tuned BERT model significantly outperforms the classic baseline, aligning with the findings in our research paper.

## **Research Paper**

The full research paper detailing the methodology, literature review, and extended results can be found in this repository:  
IMDb\_Sentiment\_Analysis\_Paper.pdf