# ATS Resume Analyzer  
**A transparent, free ATS readiness checker for job seekers**

---

## 📌 Overview

Many qualified job seekers are rejected by Applicant Tracking Systems (ATS) not because they lack skills, but because their CVs do not align with keyword-based screening criteria. Most existing ATS optimization tools are paid, opaque, or provide shallow feedback that encourages keyword stuffing.

**ATS Resume Analyzer** is a free, transparent web-based tool that helps job seekers understand how their CV matches a specific job description and provides clear, ethical recommendations on how to improve ATS visibility—without compromising human readability.

---

## 🎯 Problem Statement

Applicant Tracking Systems are widely used to filter CVs before they reach a human recruiter. These systems often rely on keyword matching, section parsing, and weighted scoring. As a result:

- Qualified candidates are filtered out early  
- Job seekers do not understand *why* they were rejected  
- Existing tools are expensive or lack transparency  

This disproportionately affects students, early-career professionals, and career switchers.

---

## 💡 Solution

This project provides a simple workflow:

1. Paste a **job description**
2. Paste a **CV (resume)**
3. Receive:
   - An ATS-style match score
   - Keyword coverage analysis
   - Missing or underrepresented skills
   - Section-based improvement suggestions

The system simulates **common ATS behavior** and explains its results clearly, helping users make informed improvements.

---

## ✨ Key Features

- ATS-style match score (0–100%)
- Required vs preferred keyword breakdown
- Missing and weak skill detection
- Section-based recommendations (Skills, Experience, Summary)
- Transparent scoring logic
- Privacy-first design (no CV data stored)
- Free and accessible

---

## 🧠 How It Works (High-Level)

- Keywords and role-specific phrases are extracted from the job description  
- The CV is analyzed using the same extraction and normalization process  
- Keywords are matched using exact, synonym, and partial matching  
- A weighted scoring model simulates common ATS filtering behavior  
- Actionable recommendations are generated for missing or weak areas  

> ⚠️ This tool does **not** represent or replicate any specific employer ATS system. It provides a realistic simulation based on widely documented ATS patterns.

---

## 🛠️ Tech Stack

**Frontend**
- React

**Backend**
- FastAPI *(or Node.js – configurable)*

**NLP & Text Analysis**
- TF-IDF
- Cosine similarity
- Keyword normalization and synonym handling

**Architecture**
- RESTful API
- Modular matching logic
- Stateless request processing

