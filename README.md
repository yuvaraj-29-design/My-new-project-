# My-new-project-
Building AI course project
# ai_text_summarizer.py

from transformers import pipeline

# Load the summarization pipeline
summarizer = pipeline("summarization")

# Input text
text = """
Artificial Intelligence (AI) is a field of computer science that aims to create machines 
that can perform tasks that would typically require human intelligence. These tasks include 
problem-solving, understanding language, recognizing patterns, learning from data, and making decisions. 
AI is transforming industries such as healthcare, finance, transportation, and education by enabling 
smarter and faster operations.
"""

# Summarize the text
summary = summarizer(text, max_length=60, min_length=25, do_sample=False)

# Print the summary
print("Summary:")
print(summary[0]['summary_text'])
# 🧠 AI Text Summarizer

This project uses a pre-trained transformer model to summarize long text passages. It was built as part of my learning journey with Google Cloud AI Certificate.

## 🔍 Description
- Input: Long text
- Output: Short, summarized version
- Model: HuggingFace Transformers (`pipeline("summarization")`)

## 📦 Technologies Used
- Python
- HuggingFace Transformers
- Pre-trained model (BART/T5)

## ▶️ How to Run
```bash
pip install transformers torch
python ai_text_summarizer.py
---

### 📎 What to Do Next:
1. Create a GitHub repo.
2. Upload:
   - `ai_text_summarizer.py`
   - `README.md`
3. Share the repo link in your resume or Google certificate submission!

---

Would you like me to:
- 🧾 Generate a **PDF certificate-style project report**?
- 🗣️ Translate the README into **Tamil**?
- 📤 Help you upload to GitHub step-by-step?

Let me know!
