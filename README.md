# Project V.O.I.C.E. AI 🚀
### Voice-Operated Infrastructure & Civic Engagement

👉 **[Live Production Web App Dashboard 🌐](https://v-o-i-c-e-ai-municipal-citizen-grievance-analytic-16396859728.asia-southeast1.run.app**

---
Project V.O.I.C.E. AI is a high-performance public governance and civic engagement backend framework built to bridge the gap between regional citizens and administrative bodies (like MP offices). 

By utilizing a lightweight, decoupled **Antigravity (Node.js/Express)** pipeline integrated with **Google AI Studio**, the system ingests unstructured regional inputs—such as conversational Tamil/Tanglish audio notes or photographic proof—and instantly processes them into clear, structured relational JSON matrices.

---

## 🌟 Key Features
*   **Grassroots Inclusivity:** Accepts conversational speech, slang, and code-switched dialects (Tanglish) to break down literacy and tech barriers.
*   **Google AI Studio Integration:** Leverages the high-speed `gemini-1.5-flash` model for unified Automatic Speech Recognition (ASR), translation, and system classification in a single pipeline pass.
*   **Privacy-First Guardrails (PII Masking):** Automatically scrubs personal data (names, contact numbers) to ensure public anonymity and compliance.
*   **Automated Severity Scoring:** Assigns an objective, mathematical urgency rank from 1 (Low) to 5 (Critical) to eliminate bureaucratic delay.

---

## 📂 Project Architecture Layout

```text
my-voice-ai-backend/
│
├── config/
│   └── aiStudioClient.js     <-- Google AI Studio SDK connection initialization
│
├── middleware/
│   └── multerConfig.js       <-- Local binary file upload interceptor
│
├── controllers/
│   └── voiceAiController.js  <-- Core AI Studio reasoning & extraction pipeline
│
├── routes/
│   └── voiceAiRoutes.js      <-- Ingestion network API endpoint mapping
│
├── uploads/                  <-- Temporary directory for buffering media data
│
├── .env                      <-- Environment keys and application server configs
└── server.js                 <-- Main application bootstrapper engine
