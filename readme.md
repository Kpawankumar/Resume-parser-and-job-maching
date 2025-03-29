# Resume parser and job Matcher

##  Overview
Resume Matcher is a Python-based tool that extracts key details from resumes (PDF/DOCX) and evaluates their compatibility with a given job description. It uses NLP techniques for information extraction and TF-IDF with cosine similarity for job matching.

## Features

- **Extracts resume text** from PDF and DOCX files.
- **Identifies Education, Experience, and Skills** using NLP and keyword matching.
- **Matches resume against job descriptions** using TF-IDF and cosine similarity.
- **Provides a Job Match Score (%)** to evaluate relevance.

## installation

!pip install spacy pdfplumber docx2txt scikit-learn
!python -m spacy download en_core_web_sm

## ussage
 run the python code in python environment
 ```
 Resume parser and job Matcher code

 ```

## How It Works
1. **Text Extraction**: Reads and cleans text from the given resume file.
2. **NLP Processing**: Uses spaCy's `en_core_web_sm` model to detect entities.
3. **Information Extraction**:
   - Education: Identifies institutions and degrees.
   - Experience: Detects timeframes.
   - Skills: Matches against a predefined skill list.
4. **Job Matching**:
   - Converts resume & job description into TF-IDF vectors.
   - Computes similarity score using cosine similarity.
   - Outputs a percentage score indicating relevance.

## Example Output
```
 Resume Details:
Education: XYZ University, Bachelor of Computer Science
Experience: 3 years experience
Skills: python, machine learning, tensorflow

 Job Match Score: 85.75%
```




## Author

**Pawan Kumar**
GitHub: [Kpawankumar][https://github.com/Kpawankumar]
