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

# Save model to clf.pkl
with open("clf.pkl", "wb") as f:
    pickle.dump(clf, f)

print("✅ Model has been trained and saved as clf.pkl")
