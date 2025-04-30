# Resume-Screening-App
Resume Screening App With Python and Machine Learning 

# how to create the clf.pkl file 
 from sklearn.datasets import load_iris
from sklearn.ensemble import RandomForestClassifier
import pickle

# Load dataset
X, y = load_iris(return_X_y=True)

# Train model
clf = RandomForestClassifier()
clf.fit(X, y)

#Save model to clf.pkl
with open("clf.pkl", "wb") as f:
    pickle.dump(clf, f)

print("✅ Model has been trained and saved as clf.pkl")


✅ What You’ll Upload to GitHub
Here’s what your GitHub repository should include:
resume-category-predictor/
│
├── app.py                             # Streamlit app
├── Resume Screening with Python.ipynb # Model training notebook
├── clf.pkl                            # Trained ML model
├── tfidf.pkl                          # TF-IDF vectorizer
├── encoder.pkl                        # Label encoder
├── requirements.txt                   # Required packages
├── README.md                          # Full documentation
├── .gitignore                         # Files to ignore
└── .gitattributes                     # For Git LFS (to handle large files)


Why We Create .pkl Files (And What They Do)
.pkl (pickle) files are used to save Python objects like models and encoders so you can reuse them without retraining every time.

🔹 Here's What Each .pkl File Does:
File	Description
clf.pkl	The trained machine learning model (e.g., Support Vector Machine) that predicts job categories based on resume text.
tfidf.pkl	The TF-IDF vectorizer that converts text into numerical features used to train and test the model.
encoder.pkl	The label encoder that converts category names into numbers and back.

