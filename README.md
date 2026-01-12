📄 AI Resume Parser & Candidate Analytics Platform
An end-to-end AI-powered Resume Parsing and Classification System built with Python, Machine Learning, and Streamlit, designed as a deployable MVP for HR analytics and talent screening.
The application extracts structured information from resumes, classifies candidates into job categories using ML, visualizes skill insights, and ranks top candidates — all deployable for free on Streamlit Cloud.

🚀 Live Demo
(Add your Streamlit Cloud URL here after deployment)

🎯 Key Features
🔍 Resume Parsing
·Extracts name, email, phone number, skills
·Supports PDF and DOCX uploads
·Handles unstructured resume text
🧠 Machine Learning Classification
·Predicts job category for each resume
·Displays confidence score (%)
·Uses a trained Scikit-Learn model
📊 Analytics Dashboard
·Skill frequency visualization
·Category-wise candidate distribution
·Interactive filtering (skills, category)
🏆 Candidate Ranking
·Top N candidates per category
·Ranked by ML confidence score
🔐 Simple Authentication (MVP)
·Session-based login system
·Ready to be replaced with full Auth in Phase 2
☁️ Cloud Ready
·Fully compatible with Streamlit Cloud
·No Docker, no FastAPI required for deployment

🧱 Tech Stack
Layer
Technology
Frontend
Streamlit
Backend Logic
Python
ML
Scikit-learn
Visualization
Plotly
File Parsing
pdfplumber, python-docx
Model Storage
joblib
Deployment
Streamlit Cloud

📁 Project Structure
resume-parser/
│
├── streamlit_app.py          # Main Streamlit application
├── requirements.txt          # Dependencies
│
├── data/
│   └── UpdatedResumeDataSet.csv
│
├── ml/
│   └── resume_classifier.pkl
│
├── utils/
│   ├── parser.py             # Resume parsing logic
│   └── file_parser.py        # PDF/DOCX extraction
│
└── README.md


⚙️ Installation & Local Setup
1️⃣ Clone the Repository
git clone https://github.com/your-username/resume-parser.git
cd resume-parser

2️⃣ Create Virtual Environment (Recommended)
python -m venv venv
venv\Scripts\activate   # Windows

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Run the App
streamlit run streamlit_app.py


☁️ Deployment on Streamlit Cloud (Free)
1.Push the project to GitHub
2.Visit 👉 https://share.streamlit.io
3.Connect your GitHub account
4.Select the repository
5.Set main file as:
streamlit_app.py

6.Click Deploy
✅ No Docker
✅ No FastAPI
✅ No paid services

🧪 Dataset & Model
·Dataset: Resume text CSV (skills & categories)
·ML Model: Multi-class classifier trained on resume text
·Output: Job category + confidence score
Model can be retrained or replaced with NLP transformers in future phases.

🔒 Authentication (Current State)
·Basic username/password (session-based)
·Designed as Phase-1 MVP
·Can be upgraded to:
oOAuth
oJWT
oDatabase-backed users

📈 Roadmap
Phase 1 (Completed)
·Resume parsing
·ML classification
·Dashboard analytics
·Free cloud deployment
Phase 2 (Planned)
·Real user authentication
·Database integration
·Resume storage
·Admin dashboard
Phase 3 (Future)
·SaaS monetization
·Resume ranking AI
·GPT-based skill extraction
·Company-level analytics

👨‍💻 Author
Muhammad Azhar
AI Engineer | AI & ML Enthusiast
📍 Pakistan
This project demonstrates real-world AI application development, SaaS thinking, and deployment skills.

📜 License
This project is licensed under the MIT License.
Free to use, modify, and distribute.

⭐ Acknowledgments
·Streamlit
·Scikit-learn
·Open-source ML community
