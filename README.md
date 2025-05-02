# Resume Classifier with NLP, ML, and Streamlit UI 🚀

A machine learning-based web application that classifies resumes into predefined job categories using Natural Language Processing (NLP). Built with Python, Scikit-learn, and Streamlit, this tool helps recruiters quickly identify candidates based on resume content.
![Screenshot 2025-04-27 200217](https://github.com/user-attachments/assets/ce47ba31-a4ca-4d32-a3e7-83f4bd6ed6bb)


---

## 📌 Features

- 📝 Upload resumes in PDF format
- 📊 Extracts and processes text data using NLP
- 🧠 Classifies resumes into job categories (e.g., Data Scientist, Web Developer, etc.)
- 🎯 Trained on labeled resume/job description dataset
- 💡 Real-time prediction via Streamlit Web UI
- 📈 Model evaluation metrics displayed (accuracy, confusion matrix)
- 📂 Simple, clean interface for quick use by HR personnel

---

## 📷 Demo

📺 **[Watch the full demo here](https://youtu.be/xSmC0lgs4ZE?si=E3nFKaJoREVMNNoR)**
![thumbnali](https://github.com/user-attachments/assets/aac39561-e379-4842-a096-a155438cb0a3)
## 🧠 How It Works

1. **Resume Upload**:
   - Users upload a PDF resume via the Streamlit UI.

2. **Text Extraction**:
   - Text is extracted from PDFs using `PyMuPDF` or `pdfminer.six`.

3. **Preprocessing**:
   - Tokenization, stopword removal, lemmatization
   - TF-IDF vectorization

4. **Classification**:
   - ML models (e.g., Naive Bayes, SVM, Logistic Regression) trained on labeled resume data
   - Predicts the job role category of the resume

5. **Output**:
   - Displays predicted category and confidence score in the Streamlit UI

---

## 🛠️ Tech Stack

- **Frontend/UI**: Streamlit
- **Backend**: Python
- **ML Framework**: Scikit-learn
- **NLP Tools**: NLTK / SpaCy
- **PDF Parsing**: PyMuPDF or pdfminer
- **Visualization**: Matplotlib, Seaborn (optional)

---
## 🎯 Use Cases
- Automate HR screening of resumes
- Categorize large volumes of resumes efficiently
- Educational demo for NLP & ML beginners

## 👤 Author;  
-  Riznee MF
- 🎓 Data Science Undergradate
- 💼 Aspiring AI/ML Engineer
- 🌐 LinkedIn | GitHub


## 📌 Tags
- NLP
- Machine Learning
- Streamlit
- Resume Classification
- Python
- Scikit-learn
- HR Tech
- PDF Processing

## NOTE(I missed to upload the clf.pkl file)
from sklearn.ensemble import RandomForestClassifier <br>
import pickle

clf = RandomForestClassifier()<br>
clf.fit(X_train, y_train)

with open('clf.pkl', 'wb') as file:<br>
    pickle.dump(clf, file)

    
