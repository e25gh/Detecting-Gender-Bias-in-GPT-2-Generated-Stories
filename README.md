# Detecting Gender Bias in GPT-2 Generated Stories  
[![GitHub](https://img.shields.io/badge/View_on-GitHub-blue?logo=github)](https://github.com/e25gh/Detecting-Gender-Bias-in-GPT-2-Generated-Stories)  

🔍 *A project analyzing gendered stereotypes in AI-generated text*  

## 🎯 Goal  
Identify if GPT-2 disproportionately associates professions (e.g., "nurse", "engineer") with specific genders.  

## 🛠️ Methods  
- Generated 50+ text samples using **Hugging Face's GPT-2**.  
- Manually analyzed outputs for gendered pronouns/assumptions.  
- Quantified bias frequency (e.g., "nurse" → 80% female pronouns).  

## 📊 Example Outputs  
| Prompt          | Generated Text (Excerpt)          | Observed Bias |  
|-----------------|-----------------------------------|---------------|  
| "The nurse..."  | "The nurse said **she** was..."   | Female        |  
| "The CEO..."    | "The CEO told **his** team..."    | Male          |  

## 🚀 How to Run  
```bash
pip install transformers torch
python bias_detection.py
