# 🚀 JobFit Analyzer - AI-POWERED RESUME SCREENING TOOL

JobFit Analyzer is a Full-Stack application that parses resumes (PDF/DOCX) and matches them against job descriptions using keyword analysis.
It provides candidates with an instant compatibility score and identifies missing skills.

## 🤜🤛 Project_Structure:-
```
ResumeAnalyzer
├── .gitignore
├── README.md
├── pom.xml                         # Backend Dependencies (Maven)
├── src/
│   ├── main/
│   │   ├── java/com/jobfitanalyzer/
│   │   │   ├── JobFitAnalyzerApplication.java  # Main Entry Point
│   │   │   ├── controller/
│   │   │   │   ├── HomeController.java
│   │   │   │   └── ResumeController.java       # API Endpoints
│   │   │   ├── exception/
│   │   │   │   └── InvalidResumeException.java
│   │   │   ├── model/
│   │   │   │   ├── Resume.java
│   │   │   │   └── ScanHistory.java            # DB Entity
│   │   │   ├── repository/
│   │   │   │   ├── resumeRepository.java
│   │   │   │   └── ScanHistoryRepository.java  # DB Operations
│   │   │   └── service/
│   │   │       ├── ResumeService.java          # Core Logic
│   │   │       └── PerformanceMonitor.java     # Multithreading
│   │   └── resources/
│   │       ├── application.properties          # DB Config
│   │       ├── static/
│   │       │   └── index.html
│   │       └── templates/
│   └── test/
│       └── java/com/jobfitanalyzer/
│           └── JobFitAnalyzerApplicationTests.java
│
└── frontend/                           # Frontend (React + Vite)
    ├── package.json                    # JS Dependencies
    ├── vite.config.ts
    ├── tailwind.config.js
    ├── postcss.config.js
    ├── tsconfig.json
    ├── public/
    │   └── vite.svg
    └── src/
        ├── main.tsx
        ├── App.tsx                     # Main Frontend Logic
        ├── App.css
        ├── index.css                   # Global Styles (Tailwind)
        └── components/
            ├── FileUpload.tsx
            ├── ResultsPage.tsx
            ├── ScannerPage.tsx
            ├── ScoreCircle.tsx
            ├── figma/                  # (Optional backup folder)
            └── ui/                     # UI Components (Shadcn)
                ├── button.tsx
                ├── select.tsx
                ├── tabs.tsx
                └── textarea.tsx
```
                

## 🌟 FEATURES
* Smart Parsing: Extracts text from both PDF (Apache PDFBox) and Word (Apache POI) documents.
* Role-Based Analysis: Pre-configured rule sets for Java, Data Analysis, Web Dev, Product Management, and DevOps.
* Gap Analysis: Instantly identifies missing keywords required for the role.
* Persistent History: Automatically saves all scan results to a local database.
* Multithreaded: Uses asynchronous processing for performance monitoring.
* Modern UI: Built with React, Tailwind CSS, and Shadcn UI.

## USER_INTERFACE:-
<img width="1256" height="636" alt="image" src="https://github.com/user-attachments/assets/36f2655e-a35a-4330-946e-3ca5b8249429" />

## DATABASE:-
<img width="1460" height="740" alt="image" src="https://github.com/user-attachments/assets/dc360908-0f84-4145-85b4-933f59b6894f" />

## RESULT_PAGE:-
<img width="1465" height="745" alt="image" src="https://github.com/user-attachments/assets/f93297be-c95a-4bd1-abf4-78c89b6c69f0" />


## 🛠️ Tech Stack
* **Backend:** Java 17, Spring Boot, Hibernate (JPA), H2 Database.
* **Frontend:** React (Vite), TypeScript, Tailwind CSS.
* **Algorithms:** Keyword Frequency & Coverage Ratio.

## 🚀 How to Run locally

### 1. Backend (Spring Boot)
1.  Open the project in IntelliJ IDEA.
2.  Run `JobFitAnalyzerApplication.java`.
3.  Server starts at `http://localhost:8081`.

### 2. Frontend (React)
```bash
cd frontend
npm install
npm run dev

📊 Example Workflow
- Upload your resume (PDF/DOCX).
- Select a job role (Java Developer, Data Analyst, etc.).
- Get an instant compatibility score.
- Review missing skills and improve your resume.
- Check scan history stored in the database.


