# Detecting Gender Bias in GPT-2 Generated Stories  
*A simple NLP project to analyze stereotypes in AI-generated text.*

## 🔍 Goal  
Identify if GPT-2 associates certain professions (e.g., "nurse", "engineer") with specific genders.  

## 🛠️ Tools Used  
- Python  
- Hugging Face Transformers (GPT-2)  

## 📋 How It Works  
1. The script generates text completions for prompts like *"The nurse said..."*.  
2. You manually review outputs for gendered language (e.g., pronouns like "she"/"he").  

## 🚀 How to Run  
1. Install dependencies:  
   ```bash
   pip install -r requirements.txt