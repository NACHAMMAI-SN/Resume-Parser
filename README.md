# Resume Parser & Job Matcher with VBA Excel Automation

A **full-stack web application** that analyzes resumes, matches them with real job listings from multiple sources, and generates **Excel reports with VBA automation tools**.

The system extracts skills from resumes, scrapes jobs from multiple platforms, calculates match percentages, and exports results into a professionally formatted Excel dashboard.

---

# Features

## Core Features

* Resume Parsing – Extract text from **PDF, DOCX, and DOC** files
* Smart Skill Detection – Detects **70+ technical skills** (Python, Java, React, AWS, VBA, etc.)
* Multi-Source Job Scraping – Fetches jobs from:

  * Naukri.com
  * Instahyre
  * RemoteOK
  * Indeed
* Intelligent Job Matching – Calculates **skill match percentage**
* Advanced Filtering – Filter jobs by location, skills, and match score

---

# Excel VBA Automation Features

## 1. Excel Report Generation

Export job matches into a **professional Excel report** containing:

* Dashboard Sheet – Summary statistics and match distribution
* Skills Sheet – All detected skills from resume
* Job Matches Sheet – Job listings with color-coded match percentages

Match colors:

* Green (70%+) – Excellent matches
* Yellow (50–69%) – Good matches
* Orange (30–49%) – Fair matches

Additional sheets:

* Top 10 Jobs – Best matching jobs ranked by relevance
* VBA Automation Tools – Built-in automation macros

---

## 2. VBA Macros (10 Built-in)

The Excel export includes **prebuilt VBA macros** for automation.

Macros included:

* FilterByMatch – Filter jobs by match %
* SortByMatchScore – Sort jobs by highest match
* HighlightTopMatches – Color-code job quality
* ExportToCSV – Export sheet to CSV
* GenerateChart – Create match distribution chart
* AutoFormatSheets – Professional formatting
* CreateSummaryStats – Generate statistics sheet
* ApplyConditionalFormatting – Format match %
* ShowNavigationMenu – Quick sheet navigation
* ExportTop10 – Export top jobs to new workbook

---

## 3. Bulk Resume Processing

Supports **processing multiple resumes at once**.

Features:

* Upload multiple resumes

* Automatic batch processing

* Consolidated Excel report including:

* Resume filename

* Email and phone

* Skills detected

* Number of jobs found

* Top 5 job matches

This is useful for **recruiters and HR teams**.

---

# Job Sources

The system collects jobs from:

* Naukri.com
* Instahyre
* RemoteOK
* Indeed

If scraping fails, a fallback job dataset is used including jobs from:

* TCS
* Infosys
* Wipro
* Accenture
* HCL
* Cognizant
* Tech Mahindra
* Capgemini

---

# Tech Stack

## Backend

* Python
* Flask
* BeautifulSoup4
* PyPDF2
* python-docx
* openpyxl
* xlsxwriter

## Frontend

* React 18
* Framer Motion
* Axios
* React Dropzone

---

# Project Structure

```
Resume-parser/
│
├── backend/
│   ├── app.py
│   ├── resume_parser.py
│   ├── job_scraper.py
│   ├── job_matcher.py
│   ├── vba_export.py
│   ├── vba_macros_template.bas
│   ├── requirements.txt
│   └── uploads/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── FileUpload.js
│   │   │   └── Results.js
│   │   ├── App.js
│   │   ├── App.css
│   │   └── index.js
│   └── package.json
│
├── Datasets/
├── start_backend.bat
└── README.md
```

---

# Installation & Running the Project

## 1. Clone the Repository

```
git clone https://github.com/Nandhana28/Resume-parser.git
```

---

## 2. Start Backend

```
cd Resume-parser/backend
python -m venv venv
venv\Scripts\activate
pip install flask flask-cors beautifulsoup4 requests PyPDF2 python-docx docx2txt openpyxl xlsxwriter selenium
python app.py
```

Backend runs at:

```
http://localhost:5000
```

---

## 3. Start Frontend

Open a **new terminal**:

```
cd Resume-parser/frontend
npm install
npm start
```

Frontend runs at:

```
http://localhost:3000
```

---

# Usage

1. Upload a resume (PDF/DOCX/DOC)
2. System extracts skills
3. Jobs are scraped from multiple sources
4. Job match percentage is calculated
5. Export results to Excel
6. Run VBA macros for automation

---

# VBA Setup

After exporting Excel:

1. Open Excel file
2. Press **Alt + F11**
3. Insert a new module
4. Copy macros from:

```
backend/vba_macros_template.bas
```

5. Save file as:

```
.xlsm (Macro-enabled workbook)
```

Run macros using:

```
Alt + F8
```

---

# Troubleshooting

### No Jobs Showing

Check backend console:

```
DEBUG: Extracted X skills
DEBUG: Got X jobs
DEBUG: Returning X jobs
```

### Excel Export Issues

Install dependencies:

```
pip install openpyxl xlsxwriter
```

Ensure backend is running on port **5000**.

---

# Future Improvements

* Add LinkedIn job scraping
* Improve AI skill detection
* Add resume scoring
* Deploy as cloud application
* Add recruiter dashboard

---

