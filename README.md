
## 🎯 Features

### 📊 Core Functionality
- **PDF Result Processing** → Extract student data from university PDF result documents  
- **Advanced Analytics** → Comprehensive performance analysis and visualization  
- **Multi-format Export** → Generate Excel, PDF, and CSV reports  
- **Responsive Design** → Works seamlessly on desktop, tablet, and mobile devices  

### 📋 Modules Overview

| Page                 | Icon | Description                                                      |
|-----------------------|------|------------------------------------------------------------------|
| Upload PDF           | 📤  | Process university result PDFs and extract student data           |
| Performance Dashboard| 📈  | Overview of class performance with metrics and trends             |
| View Top Students    | 🏆  | Identify and analyze top performers (89% and above)              |
| Division Analysis    | 📊  | Custom analysis by percentage ranges and student divisions       |
| Pass/Fail Analysis   | ✅  | Comprehensive pass/fail statistics and trends                     |
| Subject-wise Analysis| 📚  | Detailed performance analysis by individual subjects              |
| Student Search       | 🔍  | Advanced search functionality for individual student records     |
| Excel Report         | 📝  | Generate detailed Excel reports with complete student data       |

---

## 🚀 Installation Guide

### 🔧 Prerequisites
- Python **3.8 or higher**  
- `pip` (Python package manager)  
- Git (for cloning the repository)  

### 📥 Step-by-Step Installation

```bash
# 1. Clone the Repository
git clone https://github.com/your-username/college-result-management-system.git
cd college-result-management-system

# 2. Create Virtual Environment (Recommended)

# For Windows
python -m venv venv
venv\Scripts\activate

# For macOS/Linux
python3 -m venv venv
source venv/bin/activate

# 3. Install Dependencies
pip install -r requirements.txt

# 4. Run the Application
streamlit run app.py
```
The app will open in your browser at http://localhost:8501

### 📦  Requirements
| Package     | Purpose                        |
|-------------|--------------------------------|
| streamlit   | Web application framework      |
| pandas      | Data manipulation and analysis |
| matplotlib  | Data visualization             |
| pdfplumber  | PDF text extraction            |
| openpyxl    | Excel file generation          |
| fpdf        | PDF report generation          |
| numpy       | Numerical computing            |
| scipy       | Scientific computing           |
| PyYAML      | Configuration handling         |

### 🏗️ Project Structure
```bash
college-result-management-system/
├── app.py                  # Main application file
├── requirements.txt        # Python dependencies
├── .streamlit/             # Streamlit configuration
│   └── config.toml
└── pages/                  # Application modules
    ├── upload_pdf.py
    ├── dashboard.py
    ├── top_students.py
    ├── division_analysis.py
    ├── pass_fail_analysis.py
    ├── subject_analysis.py
    ├── student_search.py
    └── excel_report.py
```

## 📖 Module Documentation

### 📤 Upload PDF Module
**File:** `pages/upload_pdf.py`  
- Extracts structured student data from PDF documents using **pdfplumber** & regex  
- **Data includes:** Student info, subject-wise marks, percentages, and result status  

---

### 📈 Performance Dashboard
**File:** `pages/dashboard.py`  
- Provides class performance metrics, trends & visualizations  
- **Visuals:** Histograms, KDE plots, Pie charts  

---

### 🏆 Top Students
**File:** `pages/top_students.py`  
- Identifies students with **89%+ performance**  
- Exports ranked performer list  

---

### 📊 Division Analysis
**File:** `pages/division_analysis.py`  
- Custom analysis by percentage ranges  
- Export results in **PDF/CSV** formats  

---

### ✅ Pass/Fail Analysis
**File:** `pages/pass_fail_analysis.py`  
- Provides **subject-wise & overall pass/fail analysis**  
- Trend graphs for performance insights  

---

### 📚 Subject Analysis
**File:** `pages/subject_analysis.py`  
- Subject difficulty level analysis  
- Average score distribution  
- Performance correlation between subjects  

---

### 🔍 Student Search
**File:** `pages/student_search.py`  
- Search by **name, seat number, or filters**  
- Provides detailed student view with subject-wise performance  

---

### 📝 Excel Report
**File:** `pages/excel_report.py`  
- Generates **styled Excel reports** with student & subject data  


## 🔧 Configuration

### 📂 Streamlit Configuration (`.streamlit/config.toml`)
```toml
[server]
headless = true

[client]
showSidebarNavigation = false

[runner]
magicEnabled = false
```


