This project builds a smart Book Recommendation System that suggests books based on user preferences using Machine Learning, NLP, and Clustering techniques.
The system processes book datasets, extracts meaningful insights, and provides personalized recommendations through an interactive Streamlit web application.
🔹 Features
 Data Cleaning & Preprocessing
 Exploratory Data Analysis (EDA)
 NLP-based Feature Extraction
 Clustering (K-Means / DBSCAN)
 Recommendation Models:
Content-Based Filtering
Clustering-Based Recommendations
 Streamlit Web Interface
Optional AWS Deployment
🔹 Tech Stack
Programming: Python
Libraries:
pandas, numpy
matplotlib, seaborn
scikit-learn
nltk / sklearn NLP
Frontend: Streamlit
Deployment (Optional): AWS EC2 / S3
🔹 Dataset
Dataset 1: Audible_Catalog.csv
Contains:
Book Name
Author
Rating
Reviews
Price
Description
Genre
Listening Time
Dataset 2: Audible_Catalog_Advanced_Features.csv
Contains:
Book Name
Author
Rating
Reviews
Price
🔹 Project Workflow
1. Data Preparation
Load both datasets
Merge using Book Name + Author
2. Data Cleaning
Handle missing values
Remove duplicates
Standardize formats (genre, ratings)
3. Exploratory Data Analysis (EDA)
Genre distribution
Top authors
Ratings vs reviews
Publication trends
4. NLP Feature Extraction
Convert text (description) into vectors using:
TF-IDF / CountVectorizer
5. Clustering
Apply:
K-Means
DBSCAN
Group similar books
6. Recommendation Models
🔹 Content-Based Filtering
Based on similarity (cosine similarity)
🔹 Clustering-Based
Recommend books from same cluster
7. Model Evaluation
Precision
Recall
RMSE
8. Streamlit App
Input:
Genre / Book Name
Output:
Recommended Books
Visualization:
EDA charts
9. Deployment (Optional)
Host using AWS EC2 / S3
Project Pipeline:
Start
  ↓
Load Dataset 1 & Dataset 2
  ↓
Merge Datasets (Book Name + Author)
  ↓
Data Cleaning
  ├─ Handle Missing Values
  ├─ Remove Duplicates
  └─ Standardize Data
  ↓
Exploratory Data Analysis (EDA)
  ↓
Text Processing (NLP)
  ├─ Tokenization
  ├─ Stopword Removal
  └─ TF-IDF Vectorization
  ↓
Clustering (K-Means / DBSCAN)
  ↓
Build Recommendation Models
  ├─ Content-Based Filtering
  └─ Clustering-Based
  ↓
Model Evaluation (Precision, Recall, RMSE)
  ↓
Streamlit App Development
  ↓
User Input (Genre / Book)
  ↓
Display Recommendations
  ↓
(Optional) Deploy on AWS
  ↓
End
