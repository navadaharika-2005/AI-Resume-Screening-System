# AI Resume Screening System

An AI-powered resume screening platform that analyzes job descriptions and candidate resumes, ranks candidates using semantic similarity, and provides explainable skill-matching insights.

## Overview

Recruiters may need to review many resumes for a single job opening. Manually comparing every resume with a job description can be time-consuming.

This project uses Natural Language Processing (NLP), semantic embeddings, and cosine similarity to automatically compare resumes with a job description and rank candidates according to their relevance.

The system also identifies matched, missing, and additional skills to make the results easier to understand.

## Key Features

- Upload Job Descriptions in PDF, DOCX, or TXT format
- Upload multiple candidate resumes
- Extract text automatically from uploaded documents
- Clean and preprocess resume and job-description text
- Extract technical and soft skills using spaCy
- Generate semantic embeddings using Sentence Transformers
- Calculate resume-to-job-description similarity using cosine similarity
- Rank candidates from highest to lowest relevance
- Display matched skills
- Display missing skills
- Display additional skills
- Show an overall screening summary
- Download screening results as CSV
- Provide explainable candidate insights

## AI Pipeline

```text
Job Description
       |
       v
Text Extraction
       |
       v
Text Preprocessing
       |
       +------------------+
       |                  |
       v                  v
Skill Extraction     Semantic Embedding
       |                  |
       +--------+---------+
                |
                v
        Candidate Matching
                |
                v
       Cosine Similarity
                |
                v
       Candidate Ranking
                |
                v
    Explainable Screening Results