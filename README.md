# Resume Screening App with Python and Machine Learning

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Requirements](#requirements)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Project Structure](#project-structure)
7. [Model Training](#model-training)
8. [Contributing](#contributing)
9. [License](#license)
10. [Contact](#contact)

## Introduction
The Resume Screening App is a Python-based application designed to automate the process of screening resumes. By leveraging machine learning techniques, this app can help recruiters and HR professionals quickly identify suitable candidates based on predefined criteria.

## Features
- Extracts text from various resume formats (PDF, DOCX, TXT).
- Analyzes and scores resumes based on relevant skills and experiences.
- Provides a user-friendly interface for uploading and reviewing resumes.
- Generates detailed reports on candidate suitability.

## Requirements
- Python 3.8+
- Libraries: 
  - `streamlit`
  - `pickle`
  - `re`
  - `nltk`
  - `scikit-learn`

## Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/Resume-Screening-App.git
   cd Resume-Screening-App
   ```

2. **Create a virtual environment and activate it:**
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`
   ```

3. **Install the required packages:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Download NLTK data:**
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   ```

## Usage
1. **Run the Streamlit web application:**
   ```bash
   streamlit run app.py
   ```

2. **Open your web browser and navigate to:**
   ```
   http://localhost:8501/
   ```

3. **Upload resumes and review the screening results.**

## Project Structure
```
Resume-Screening-App/
│
├── app.py                # Main application file
├── resume_read.ipynb     # Notebook for reading and processing resumes
├── clf.pkl               # Trained classification model
├── tfidf.pkl             # TF-IDF vectorizer model
├── requirements.txt      # List of dependencies
└── README.md             # Project documentation
```