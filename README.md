# Detecting Gender Bias in GPT-2 Generated Stories  
[![GitHub](https://img.shields.io/badge/View_on-GitHub-blue?logo=github)](https://github.com/e25gh/Detecting-Gender-Bias-in-GPT-2-Generated-Stories)  
🔍 *An NLP project uncovering stereotypes in AI-generated text*

## 🎯 Goal  
Identify whether GPT-2 disproportionately associates professions (e.g., "nurse", "engineer") with specific genders.

## 🛠️ Methods  
- Generated 100+ text samples using **Hugging Face's GPT-2**  
- Analyzed outputs for:  
  - Gendered pronouns ("she" vs. "he")  
  - Stereotypical role assignments  
- Quantified bias frequency per profession  

## 📊 Example Outputs  
| Prompt          | Generated Text Excerpt          | Female Terms | Male Terms |
|-----------------|--------------------------------|-------------|-----------|
| "The nurse..."  | "The nurse said **she** was..." | 3           | 0         |
| "The CEO..."    | "The CEO told **his** team..."  | 0           | 2         |

```python
# Sample bias distribution (simulated)
import matplotlib.pyplot as plt
professions = ["Nurse", "Engineer", "CEO"]
bias_score = [85, 15, 20]  # % female-associated
plt.bar(professions, bias_score)
plt.title("Profession-Gender Association in GPT-2")
