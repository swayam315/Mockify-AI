Mockify AI — README.md
⭐ Overview
**Mockify AI is an advanced mock interview platform designed to help users practice both coding and HR-style interview rounds with an intelligent AI experience.**

**Current system capabilities include:**
-AI-assisted coding interview simulation
-Scoring, complexity analysis, and technical feedback
->HR/behavioral Q&A interactions
->Modern user interface with pricing, about, login, and dashboard views

The platform is 75% complete, and upcoming versions will include a connected backend & enhanced features to make it fully robust.

📁 Project Structure
index.html        → Landing page  
aboutus.html      → About & roadmap  
interview.html    → Coding + HR interview interface  
price.html        → Pricing page  
style.css         → Custom styles  
script.js         → UI logic, auth behavior, config handling

⚙ Setup Instructions

Place all project files in one folder.

(Optional) Add Firebase config if you want auth enabled:

<script>
  window.__firebase_config = JSON.stringify({
    apiKey: "YOUR_KEY",
    projectId: "YOUR_PROJECT"
  });
</script>


Run any local server:

python3 -m http.server 8000


Open http://localhost:8000

Use demo login credentials: admin / admin123

🏗 Architecture Overview

Core system built using HTML, TailwindCSS, JavaScript

AI-driven features use a function such as callGemini()

Backend endpoints will be integrated soon to make the entire flow fully functional

Designed with scalability in mind: user accounts, progress tracking, and advanced analytics will be integrated in the next phases

▶ How to Run an Interview Session

Login → Open Start Interview

Choose HR or Coding challenge

Submit your answer

The system returns structured AI feedback:

SCORE: 0–100
COMPLEXITY: O(n)
FEEDBACK: Brief technical review

🔌 Backend Endpoints (Planned Integration)

To complete the system’s backend development:

POST /api/gemini

Handles AI responses for coding & HR questions.
Expected output format:

SCORE: ...
COMPLEXITY: ...
FEEDBACK: ...

POST /api/login

Authenticates users and manages dashboard access.

These integrations will make the platform production-ready.

📦 Dependencies

TailwindCSS

Lucide Icons

Google Fonts

Firebase (optional)

👥 Contributors

Swayam Khangaonkar — AI

Omkar S — Product & Design

Sarthak Chillal — Frontend

Aakash Iti — Backend
