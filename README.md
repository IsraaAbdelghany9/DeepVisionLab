# DeepVisionLab

A comprehensive collection of AI projects and experiments exploring machine learning, deep learning, computer vision, natural language processing, and large language models. This repository serves as a personal research lab where concepts are tested, models are built, and ideas are transformed into intelligent systems.

## Repository Structure

This repository contains projects organized by domain:

### Computer Vision
Image classification, object detection, and computer vision projects including:
- Potato Disease Leaf Classification
- Image Classification Examples

### Deep Learning
Neural network architectures, ANNs, CNNs, LSTMs, and deep learning models including:
- Credit Score prediction with ANNs
- Deep Learning Models on CIFAR-10 & MNIST
- Fruits classification
- MNIST with LSTM
- U-Net model implementations
- Diabetes prediction with ANN

### Machine Learning
Classical ML algorithms including regression, classification, and clustering:
- California Real Estate Analysis
- Multiple Linear Regression, Ridge, Lasso on Hitters Dataset
- Credit Card Classification with SVM variants
- Decision Trees implementations

### Natural Language Processing
Text processing, sentiment analysis, and NLP applications:
- Twitter Sentiment Analysis
- Hate Speech Classification
- Various NLP assignments

### Large Language Models
LLM integration, LangChain tutorials, and generative AI projects. This section houses a collection of diverse projects leveraging Large Language Models (LLMs) with focus on prompt engineering, fine-tuning, and integrating LLMs while creating practical and innovative applications.

#### LLM Notebooks:

1. `001_website_scrapping_summerizing`
    - A small project that scrapes given URL and summarizes it
    - Can be added in a larger task later on 

2. `002_LangChain_Tutorial`
    - Starting with langchain and testing its code with Gemini 
    - Based on documentation from [langchain_google_generative_ai](https://python.langchain.com/docs/integrations/chat/google_generative_ai/)

3. `003_LangChain_Tutorial_2`
    - Explores PromptTemplate from langchain_core 
    - Can be used in all other projects - easier to use when you have variables in the prompt

4. `004_LinkedIn_Scraping` 
    - Scrapes LinkedIn profiles using URL, gets info and summarizes it using LLM 
> To get the API key check: [Scrapin](https://app.scrapin.io/api)

5. `005_llama_with_langchain`
    - Integration of Llama models with LangChain

6. `006_langgraph_tutorial_1`
    - Tutorial on using LangGraph for building complex LLM workflows

#### Helper Scripts 

##### gemini_models_print.py

Helper script to print available Gemini models. Can be edited to filter specific models:

```python
for model in models:
    if "flash" in model.name:
        print(model.name)

## OR

for model in models:
    if model.name.endswith("generation"):
        print(model.name)
```

#### Note About Black and nbqa

- **🖤 Black** is a **Python code formatter** that automatically formats your code to follow best practices (PEP8), making it clean and consistent.

- **📓 nbqa** lets you use **Black (and other tools)** directly on **Jupyter Notebooks** (`.ipynb`), applying formatting to code cells while preserving markdown and outputs.

✅ Use `black` for `.py` files  
✅ Use `nbqa black` for `.ipynb` files
