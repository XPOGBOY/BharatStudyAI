# BharatStudy AI – System Design Document

## 1. Architecture Overview

BharatStudy AI follows a modular AI-assisted web architecture:

Frontend (React/Next.js)
        |
Backend API (FastAPI)
        |
AI Processing Layer
        |
Database + File Storage
        |
AWS Cloud Deployment

---

## 2. System Components

### 2.1 Frontend Layer

Technology:
- React or Next.js

Responsibilities:
- User authentication (basic session)
- File upload interface
- Form submission
- Dashboard display
- Resume preview
- Interview chat interface

---

### 2.2 Backend Layer

Technology:
- Python FastAPI

Responsibilities:
- Handle API requests
- Process file uploads
- Connect to AI services
- Generate structured responses
- Return formatted outputs

Endpoints (MVP):

POST /predict-exam
POST /skill-gap
POST /generate-resume
POST /interview-session

---

### 2.3 AI Processing Layer

Components:

1. NLP Engine
   - Text extraction
   - Keyword frequency detection
   - Pattern recognition

2. LLM Integration
   - Question generation
   - Resume rewriting
   - Interview question generation
   - Feedback evaluation

3. Scoring Engine
   - Keyword matching
   - Similarity scoring
   - Basic evaluation heuristics

---

### 2.4 Database

Technology:
- MongoDB / Firebase

Stores:
- User sessions
- Resume analysis results
- Interview history
- Roadmap data

---

### 2.5 File Storage

Technology:
- AWS S3

Stores:
- Uploaded syllabus files
- Resume PDFs
- Generated resume outputs

---

## 3. Data Flow

### Exam Prediction Flow

1. User uploads syllabus
2. Backend extracts text
3. NLP engine analyzes keywords
4. LLM generates structured questions
5. Output displayed on dashboard

---

### Skill Gap Flow

1. Resume uploaded
2. Resume parsed
3. Compared with job role template
4. Missing skills identified
5. Roadmap generated

---

### Resume Builder Flow

1. User enters details
2. LLM rewrites content
3. Structured resume template applied
4. PDF generated and returned

---

### Interview Simulation Flow

1. Role selected
2. Questions generated
3. User submits answers
4. AI evaluates response
5. Feedback + score returned

---

## 4. Security Design

- HTTPS enforced
- Temporary file storage
- No permanent resume storage (optional)
- API rate limiting

---

## 5. Scalability Plan

- Stateless backend
- Containerized deployment
- Auto-scaling EC2
- Modular AI service calls

---

## 6. AWS Deployment Plan

- Frontend: AWS Amplify
- Backend: EC2 or AWS Lambda
- Storage: S3
- Database: MongoDB Atlas
- API Gateway (optional)

---

## 7. Design Principles

- Simple UI
- Modular AI services
- Clear separation of concerns
- Scalable cloud-first design
- Low-bandwidth optimized responses
