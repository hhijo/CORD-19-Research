# 📘 CORD-19 Data Explorer

This project explores the **CORD-19 metadata dataset** using Python (pandas, matplotlib, seaborn, wordcloud) and an interactive **Streamlit application**. The goal is to practice **data loading, cleaning, analysis, visualization, and app deployment**.

---

## 📂 Project Structure
```
CORD19-Explorer/
│── metadata.csv              # Dataset (not included here due to large size)
│── Metadata.ipynb            # Jupyter Notebook with data wrangling & analysis
│── app.py                    # Streamlit application
│── README.md                 # Documentation
```

---

## ⚙️ Installation & Setup

1. **Clone the repository** (or download the files)
   ```bash
   git clone https://github.com/hhijo/CORD-19-Research.git
   cd CORD-19-Research
   ```

2. **Install dependencies**
   ```bash
   pip install pandas matplotlib seaborn wordcloud streamlit
   ```

3. **Run Jupyter Notebook (optional)**
   ```bash
   jupyter notebook Metadata.ipynb
   ```

4. **Launch the Streamlit App**
   ```bash
   streamlit run app.py
   ```

---

## 🧾 Workflow

### Part 1: Data Loading & Exploration
- Loaded `metadata.csv` into a pandas DataFrame.
- Explored dataset dimensions, data types, and missing values.
- Generated descriptive statistics for numeric columns.

### Part 2: Data Cleaning & Preparation
- Removed columns with **>80% missing values**.
- Converted `publish_time` column to datetime.
- Extracted **year** from `publish_time`.
- Created a new feature: **abstract word count**.

### Part 3: Data Analysis & Visualization
- Counted publications by year.
- Identified **top publishing journals**.
- Extracted most frequent words in titles using simple word frequency.
- Created visualizations:
  - Bar chart: publications over time.
  - Horizontal bar chart: top journals.
  - Word cloud: paper titles.
  - Bar chart: distribution of papers by source.

### Part 4: Streamlit Application
- Built an interactive app with:
  - Year range slider for filtering.
  - Sample data preview.
  - Bar charts for yearly publications and journals.
  - Word cloud for paper titles.

### Part 5: Documentation & Reflection
- Documented workflow, code, and results.
- Reflected on challenges and key learnings.

---

## 📊 Sample Visualizations
- **Publications per year** (trend of COVID-19 research)
- **Top Journals** publishing COVID-19 research
- **Word Cloud** of paper titles
- **Distribution by Source**

---

## 🔍 Reflections
- **Challenges:**  
  - The dataset is very large, making it slow to load.  
  - Many missing values across columns (had to drop or clean).  
  - Text data (titles/abstracts) required preprocessing for word analysis.  

- **Learnings:**  
  - Gained hands-on experience with **pandas data cleaning**.  
  - Learned to use **word clouds** and **basic text analysis**.  
  - Improved skills in building simple dashboards with **Streamlit**.  
  - Understood how to move from raw data → insights → interactive app.  

---

## 🚀 Future Work
- Apply **NLP techniques** (topic modeling, sentiment analysis).  
- Integrate **interactive filters** (by journal, author, country).  
- Deploy the app online using **Streamlit Cloud** or **Heroku**.  
