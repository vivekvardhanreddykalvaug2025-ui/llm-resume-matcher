LLM-Powered Resume Matcher and Score Evaluator

## Overview

Recruiters often spend a significant amount of time reviewing resumes, and traditional keyword-based screening can overlook qualified candidates. This project explores how Natural Language Processing (NLP), semantic search, and Large Language Models (LLMs) can improve resume screening.

The system processes 5,000 resumes and matches them against 10 sample job descriptions. Using Sentence Transformers and ChromaDB, it retrieves the most relevant resumes through semantic search. The shortlisted candidates are then evaluated by an LLM across skills, experience, education, domain relevance, keyword match, and resume quality. Finally, the system generates an ATS-style evaluation report, calculates an overall match score using weighted scoring, identifies skill gaps, and ranks candidates.

---

## Features

- Resume preprocessing and cleaning
- Semantic search using Sentence Transformers and ChromaDB
- Cosine similarity-based resume retrieval
- LLM-based candidate evaluation
- ATS-style evaluation report
- Weighted candidate ranking
- Skill gap analysis

---

## Workflow

1. Preprocess resume data.
2. Generate sentence embeddings.
3. Store embeddings in ChromaDB.
4. Retrieve relevant resumes using semantic search.
5. Evaluate shortlisted candidates with an LLM.
6. Generate ATS-style reports, calculate match scores, and rank candidates.


## Tech Stack

- Python
- Pandas
- Scikit-learn
- NumPy
- Sentence Transformers (`all-MiniLM-L6-v2`)
- ChromaDB

- Groq API
- llama-3.1-8b-instant
- Jupyter Notebook
-python-dotenv


## Scoring Criteria

| Category | Weight |
|--------------------|-------:|
| Skills Match | 35% |
| Experience Match | 25% |
| Education Match | 10% |
| Domain Relevance | 15% |
| Keyword Match | 10% |
| Resume Quality | 5% |

## Visualization 
Several visualization techniques were used to analyse and interpret the performance of the proposed resume screening system. 
Cosine Similarity Heatmap: Visualizes the semantic similarity between candidate resumes and selected job descriptions, demonstrating the effectiveness of vector-based retrieval.  
Candidate Ranking Bar Chart: Displays the final match scores of shortlisted candidates for each job description, enabling recruiters to compare candidate suitability visually



## Learning Outcome

Working on this project helped us understand how semantic search and LLMs can be combined to solve a real-world problem. We gained hands-on experience with text preprocessing, sentence embeddings, vector databases, prompt engineering, and building an end-to-end NLP pipeline. It also improved our understanding of designing evaluation systems and interpreting ATS-style candidate assessments.


## Future Improvements

- Build a Streamlit web application
- Support PDF resume uploads
- Add an interactive recruiter dashboard
- Experiment with different embedding models and LLMs


## Contributors

- Vivek Vardhan Reddy Kalva
- Katnam Sri Satya Pranathi

