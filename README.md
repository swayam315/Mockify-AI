# Mockify AI

---

## ⭐ Overview

Mockify AI is a modern mock interview platform built to help users practice *coding rounds* and *HR-style interviews* with intelligent AI assistance.

Current version is *~85% complete* and already supports:

- AI-assisted *coding interview simulation*
- *Score, complexity & feedback* generation
- *HR / behavioral Q&A* interactions
- Modern UI with *pricing, about, login & dashboard*

Upcoming development will include backend connectivity, user accounts, analytics, and added robustness.

---

## 📁 Project Structure


index.html        → Landing page  
aboutus.html      → About & roadmap  
interview.html    → Coding + HR interface  
price.html        → Pricing section  
style.css         → Custom styles  
script.js         → UI logic, authentication handling, config loading


---

## ⚙ Setup Instructions

1. Place all project files in one folder.  
2. (Optional) Add Firebase config for authentication features:
   html
   <script>
     window.__firebase_config = JSON.stringify({
       apiKey: "YOUR_KEY",
       projectId: "YOUR_PROJECT"
     });
   </script>
   
3. Start a local dev server:
   bash
   python3 -m http.server 8000
   
4. Visit: http://localhost:8000  
5. Use demo credentials: *admin / admin123*

---

## 🏗 Architecture Overview

- Built using *HTML, **TailwindCSS, and **JavaScript*  
- AI-powered features call a function like callGemini() for dynamic responses  
- Backend endpoints will be integrated in the next development phase  
- Designed for scalability and future enhancements (user accounts, history tracking, analytics)

---

## ▶ How to Run an Interview Session

1. Login and navigate to *Start Interview*  
2. Choose coding or HR mode  
3. Submit your answer  
4. AI returns structured feedback, example:


SCORE: 82
COMPLEXITY: O(n)
FEEDBACK: The solution is efficient but lacks edge-case handling...


---

## 🔌 Planned Backend Endpoints

### POST /api/gemini
Handles AI analysis for coding & HR responses.  
Expected response format:

SCORE: ...
COMPLEXITY: ...
FEEDBACK: ...


### POST /api/login
Authenticates users and manages sessions.

These will complete the platform’s transition to a fully robust production system.

---

## 📦 Dependencies

- TailwindCSS  
- Lucide Icons  
- Google Fonts  
- Firebase (optional for auth)

---

## 👥 Contributors

- *Swayam Khangaonkar* — AI  
- *Omkar S* — Product & Design  
- *Sarthak Chillal* — Frontend  
- *Aakash Iti* — Backend  

---
