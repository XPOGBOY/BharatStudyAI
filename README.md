# BharatStudy AI – Requirements Document

## 1. Project Overview

BharatStudy AI is an India-first AI-powered exam and career assistant designed to help students:

- Predict important exam questions
- Identify skill gaps for job roles
- Generate ATS-friendly resumes
- Practice AI-based mock interviews

The platform focuses on Indian university syllabi and placement ecosystems.

---

## 2. Problem Statement

Indian students face:

- Uncertainty about important exam topics
- Lack of structured placement preparation
- Poor resume optimization for ATS systems
- No personalized interview feedback tools

Existing AI tools are generic and not aligned with Indian academic patterns or entry-level hiring trends.

---

## 3. Target Users

- B.Tech / B.Sc / BCA students
- Final-year students preparing for placements
- Tier-2 and Tier-3 college students
- Freshers entering job market

---

## 4. Functional Requirements

### 4.1 Exam Prediction Engine

Input:
- Syllabus (PDF or text)
- Optional past year papers

Output:
- Top predicted questions (unit-wise)
- Short model answers (3–5 bullet points)
- 7-day revision plan

Requirements:
- Extract text from PDF
- Identify repeated keywords
- Generate structured questions
- Provide concise answers

---

### 4.2 Skill Gap Detector

Input:
- Resume upload (PDF)
- Selected job role (predefined list)

Output:
- Missing skills
- Strength areas
- 30-day roadmap
- Learning recommendations

Requirements:
- Resume parsing
- Keyword matching against job template
- Similarity scoring logic
- Roadmap generation

---

### 4.3 AI Resume Builder

Input:
- User profile details
- Skills and projects

Output:
- ATS-friendly formatted resume
- Improved bullet points
- Downloadable PDF file

Requirements:
- Rewrite using strong action verbs
- Format in clean single-template layout
- Export as PDF

---

### 4.4 AI Interview Simulator

Input:
- Selected role
- Experience level

Output:
- 5–7 generated interview questions
- Text-based answer submission
- AI-generated feedback
- Performance scoring

Requirements:
- Question generation logic
- Feedback evaluation system
- Scoring mechanism

---

## 5. Non-Functional Requirements

- Web-based application
- Responsive UI
- Secure file upload handling
- Lightweight performance
- Cloud deployment (AWS)

---

## 6. Constraints

- Limited to predefined job roles in MVP
- English language support (Hindi optional)
- No real-time job scraping
- Text-based interviews only (voice future scope)

---

## 7. Success Criteria

- Accurate and structured question prediction
- Meaningful skill gap identification
- Resume clarity improvement
- Realistic interview simulation feedback

---

## 8. Future Enhancements

- Multi-language support
- Voice-based interview simulation
- Real-time job scraping integration
- University-specific syllabus database
- Mobile application
