# ATS Resume–JD Matcher

### Overview

The ATS Resume–JD Matcher is a Python Flask application that evaluates the compatibility between a candidate’s resume and a job description. Using NLP techniques and cosine similarity, it calculates a match score, helping applicants understand how well their resume aligns with a given job posting.

This project demonstrates NLP preprocessing, ML-based text similarity, and simple web deployment, making it ideal for students and professionals exploring applied AI in recruitment technologies.

---
### Features

- Upload **resume (PDF)** and **job description (PDF)** for analysis
- **Text extraction** from PDF files using PyPDF2
- **Text cleaning & preprocessing** with SpaCy (lowercasing, lemmatization, stop-word and punctuation removal)
- **TF-IDF vectorization** and **cosine similarity** scoring to quantify resume-job fit
- Simple and clean **Flask web interface** for real-time interaction
- Outputs a match **percentage score**

---
### Demo

Upload a resume and JD PDF to see the match score instantly.

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/79089f10-28ed-4617-bb02-92f7fe006720" />


---
### Installation

1. Clone the repository:
```
git clone https://github.com/your-username/ats-resume-matcher.git
cd ats-resume-matcher
```

2. Install dependencies:
```
pip install -r requirements.txt
python -m spacy download en_core_web_lg
```

3. Run the Flask app:
```
python app.py
```

4. Open your browser and navigate to:
```
http://127.0.0.1:5000
```
---
### Usage

1. Upload your **resume PDF**.
2. Upload the **job description PDF**.
3. Click **“Check Match”.**
4. The app displays a **compatibility score (%)**, indicating how closely your resume matches the job description.

---
### Technologies Used

- **Python** – Programming and ML scripting
- **Flask** – Web app framework
- **PyPDF2** – PDF text extraction
- **SpaCy** – NLP preprocessing (lemmatization, stop-word removal)
- **Scikit-learn** – TF-IDF vectorization & cosine similarity

---
### Project Structure
```
ats-resume-matcher/
├─ app.py
├─ requirements.txt
├─ templates/
│   └─ home.html
└─ README.md
```

---
### Future Work

- Enhance **UI/UX** for better user experience
- Support **multiple file formats** (docx, txt)
- Implement **batch resume scoring** for recruiters
- Integrate with a **dashboard** to visualize matching analytics
- Explore **semantic similarity** using **transformer models** (BERT, RoBERTa) for more accurate scoring

---
### License

This project is for educational purposes. You can modify and use it for personal learning or portfolio demonstrations.
