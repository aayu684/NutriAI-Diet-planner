# 🍽️ NutriAI — AI-Powered Diet Planner  

**NutriAI** is a modern, responsive web application that leverages the power of **Google’s Gemini API** to generate **personalized 7-day diet plans**.  
It combines the efficiency of a **React + TypeScript** frontend with a secure **Python (Flask/FastAPI)** backend to deliver scientifically balanced, goal-oriented meal schedules — focused on **Indian cuisine**.

---

## 🧠 Overview  

NutriAI provides users with customized meal recommendations based on individual details such as age, height, weight, fitness goals, and dietary preferences.  
By integrating the **Gemini AI model**, the backend intelligently generates daily meal plans that are nutritionally balanced, allergy-aware, and culturally relevant.  

---

## 🏛️ Architecture  

This project follows a modern **client-server architecture**:

| Layer | Description |
|--------|-------------|
| **Frontend (Client)** | Built with **React, TypeScript, and Tailwind CSS**, the frontend is a single-page application (SPA) that collects user inputs and displays the AI-generated 7-day plan. It never exposes the Gemini API key. |
| **Backend (Server)** | A **Python Flask/FastAPI** service that securely stores the Gemini API key, receives user data from the frontend, builds structured prompts, calls the **Google Gemini API**, and returns the generated plan in JSON format. |

---

## 🚀 Features  

✨ **Secure API Key Management** – API key is stored safely in backend `.env`, never exposed to the browser.  
👤 **Personalized Inputs** – Collects user name, age, height, weight, activity level, goals, and preferences.  
🚫 **Allergy-Aware** – Automatically avoids ingredients that match user allergies.  
🤖 **AI-Powered Generation** – Uses **Google Gemini API** to dynamically build 7-day meal plans based on Indian food data.  
🧩 **Structured Output** – Ensures valid JSON response using a strict backend schema.  
📱 **Responsive Design** – Clean, mobile-first interface built with Tailwind CSS.  

---

## 🛠️ Tech Stack  

| Component | Technology |
|------------|-------------|
| **Frontend** | React, TypeScript, Tailwind CSS, Vite |
| **Backend** | Python, Flask/FastAPI, Google Gemini API |
| **Deployment** | Vite Dev Server (Frontend) + Flask API (Backend) |
| **Data** | Indian food dataset (Calories, Protein, Carbs, Fats) |

---


---

## ⚙️ Setup Instructions  

### 🧩 Prerequisites
- Node.js (v18 or newer)  
- Python (v3.9 or newer)  
- A valid **Google Gemini API Key** (get from [Google AI Studio](https://aistudio.google.com/))

---

## 🧩 API Workflow  

1️⃣ **Frontend collects** user details and goals.  
2️⃣ **Sends a POST request** to `http://localhost:5000/api/generate-plan`.  
3️⃣ **Backend builds** a structured AI prompt using user data and Indian food dataset.  
4️⃣ **Gemini API generates** a complete 7-day diet plan.  
5️⃣ **Backend returns structured JSON**, which the frontend displays as a weekly table.  

---

## ⚠️ Disclaimer  

> This application is for **informational and educational purposes only**.  
> It is **not a substitute for professional medical or dietary advice**.  
> Always consult a certified nutritionist or healthcare professional before making major dietary changes.  

---

## ✨ Made by  

**Aayushi Soni**  
🎓 B.Tech in Computer Engineering | Data Science & AI Enthusiast  
