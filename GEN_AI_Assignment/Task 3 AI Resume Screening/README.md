🧠 AI Resume Screening System (LangChain + Groq)

📌 Overview

This project is an AI-powered Resume Screening System that evaluates candidates based on a given job description.
It follows a structured pipeline to extract, match, score, and explain candidate suitability.

---

⚙️ Tech Stack

- Language: Python
- Framework: LangChain (LCEL)
- LLM Provider: Groq API
- Model Used: "llama3-8b-8192" (or updated Groq model like "llama3-8b-instant")
- Tracing: LangSmith

---

🔄 Pipeline Architecture

Resume → Extraction → Matching → Scoring → Explanation

---

🚀 Features

- Extracts skills, experience, tools, and education from resumes
- Matches candidate profile with job requirements
- Assigns a score (0–100)
- Provides hiring recommendation (Strong Hire / Consider / Reject)
- Generates explanation for decision
- Supports Few-Shot Prompting for improved accuracy
- LangSmith tracing enabled for debugging

---

📊 Test Cases

- ✅ Strong Candidate
- ⚖️ Average Candidate
- ❌ Weak Candidate


---

🔑 Setup

1. Get Groq API key
2. Add to ".env":

GROQ_API_KEY=your_key_here
LANGCHAIN_TRACING_V2=true

---

▶️ Run

Execute all cells in the Jupyter Notebook to see:

- Extraction
- Matching
- Scoring
- Explanation
- Final Results

---

📌 Output Example

STRONG → 75  
AVERAGE → 50  
WEAK → 0  

---

✨ Notes

- Strict JSON output enforced
- No hallucinated skills (only resume-based evaluation)
- Modular and clean implementation

---

