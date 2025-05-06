# Job Matching Intelligence and Automation

A modular pipeline for crawling, extracting, analyzing, and automating job application content from Google Jobs — enhanced by Large Language Models.

---

## What This Project Does

- Scrape job listings from **Google Jobs**  
- Clean & extract structured information from unstructured text  
- Analyze job trends using **EDA & NLP**  
- Auto-generate **personalized resumes & cover letters** using LLMs

---

## How It Works

### 1. Job Data Collection
- Uses [SerpAPI](https://serpapi.com/google-jobs-api) to scrape job listings across roles, sectors, and locations
- API supports structured job fields like title, company, salary, and raw description

### 2. Data Cleaning & Structuring
- Extracts and standardizes:
  - Job title, company, industry, location
  - Job type, salary range, experience, skills, responsibilities
  - Remote status, company size, deadline
- Output: `data/processed-jobs-1.csv`

### 3. LLM-based Smart Extraction
- Applies LLM APIs (e.g., OpenAI) to automate job parsing and feature tagging  
- Uses **prompt engineering** to reliably extract key fields from natural language

### 4. Exploratory Data Analysis
- Visualizes:
  - Distribution of job titles, types, and salaries
  - Salary vs. experience/location
  - Keyword trends and semantic clustering via NLP
  - Geographic job spread using Folium maps

### 5. Resume & Cover Letter Generator
- Automatically generates customized application materials for each job
- Uses LLM + [Quarto](https://quarto.org/) to render HTML or PDF documents

---

## Tech Stack

| Component            | Tool/Library                 |
|---------------------|------------------------------|
| Scraping            | `serpapi`, `requests`        |
| Data Handling       | `pandas`, `numpy`            |
| Visualization       | `matplotlib`, `seaborn`, `folium` |
| NLP & Automation    | `openai`, `nltk`, `spacy`, `scikit-learn` |
| Doc Generation      | `quarto`, `jinja2`, `markdown` |
| Environment Config  | `python-dotenv`              |

---


