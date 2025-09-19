# 🧑‍💼 Smart Resume Analyzer (SRA)

Smart Resume Analyzer (SRA) is an **AI-powered resume analysis web application** built with **Streamlit**.  
It analyzes resumes, extracts skills & information, recommends improvements, suggests courses, and even provides bonus career guidance videos 🎥.  

---

## ✨ Features

- ✅ **Upload Resumes (PDF)** – Extracts name, email, skills, experience, and number of pages  
- ✅ **Resume Analysis** – Evaluates candidate level (Fresher, Intermediate, Experienced)  
- ✅ **Skills Extraction & Recommendation** – Detects existing skills and suggests additional industry-relevant skills  
- ✅ **Career Path Prediction** – Identifies suitable career fields:
  - Data Science  
  - Web Development  
  - Android Development  
  - iOS Development  
  - UI/UX Design  
- ✅ **Course Recommendations 🎓** – Curated learning paths & certifications  
- ✅ **Resume Writing Feedback** – Evaluates Objective, Declaration, Hobbies, Achievements, Projects  
- ✅ **Resume Score** – A dynamic progress bar showing resume completeness  
- ✅ **Video Resources** – Auto-recommended YouTube videos for Resume Writing & Interview Preparation  
- ✅ **Admin Dashboard** –  
  - View all user data in tabular format  
  - Download user reports (CSV)  
  - Visual analytics (Pie charts for Predicted Fields & Candidate Levels)  

---

## 🛠️ Tech Stack

- **Frontend / UI**: [Streamlit](https://streamlit.io/)  
- **Backend / Resume Parsing**: [pyresparser](https://github.com/OmkarPathak/pyresparser), [pdfminer3](https://pypi.org/project/pdfminer3/)  
- **Database**: MySQL (`pymysql`)  
- **Visualization**: [Plotly](https://plotly.com/python/)  
- **NLP**: NLTK, spaCy  
- **Others**: Pafy, youtube-dl, PIL, Base64, Random, Pandas  

---

## 📂 Project Structure

Smart_Resume_Analyzer/
├── Logo/
│ ├── SRA_Logo.ico
│ └── SRA_Logo.jpg
├── Uploaded_Resumes/ # Stores uploaded resumes
├── Courses.py # Course & video recommendation data
├── app.py # Main Streamlit Application
├── requirements.txt # Python dependencies
└── README.md
---
## 2️⃣ Install dependencies

Make sure you have Python 3.8+ installed.

pip install -r requirements.txt

If requirements.txt is missing, install manually:

pip install streamlit nltk spacy pandas pyresparser pdfminer3 pymysql streamlit-tags pafy youtube_dl plotly Pillow

3️⃣ Download NLP Models
python -m nltk.downloader stopwords
python -m spacy download en_core_web_sm

4️⃣ Setup Database (MySQL)

Start MySQL and create database & table automatically by running the app.
Default connection inside code:

connection = pymysql.connect(host='localhost', user='root', password='')


➡️ Update credentials if needed.

5️⃣ Run the Application
streamlit run app.py

6️⃣ Access App

Open browser → http://localhost:8501

🔑 Admin Login

To access the Admin Dashboard:

Username: machine_learning_hub

Password: mlhub123

📊 Admin Dashboard Features

View all user records

Download data as CSV

Pie-chart analytics:

Predicted Career Fields

User Experience Levels

🎥 Demo Flow

Upload a resume (PDF)

View extracted information (Name, Email, Skills, Pages)

Get Candidate Level (Fresher / Intermediate / Experienced)

Receive Recommended Skills & Courses

View Resume Writing Tips & Score

Watch Resume + Interview Preparation Videos

Admin can log in to view analytics & download reports

📜 License

This project is licensed under the MIT License.
You’re free to use, modify, and distribute it.

👨‍💻 Author

Developed with ❤️ by Vijeth Naik

