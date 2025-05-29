# Viksitai Project

Viksit.AI is a full-stack project built with **Django** for the backend and **React (Vite)** for the frontend. It leverages various third-party APIs to provide AI assistance, search functionality, and code execution support.

---

## 🔐 API Key Configuration

This project uses multiple third-party APIs. To run it locally, you need to configure API keys in `.env` files for both the **backend** and **frontend**.

### ✅ Backend (`backend/.env`)

Create a `.env` file inside the `backend/` directory and add the following keys:

- `GROQ_API_KEY`
- `GOOGLE_API_KEY`
- `GOOGLE_CSE_ID`
- `SARVAM_API_KEY`
- `DJANGO_SECRET_KEY`
- `GITHUB_TOKEN`
- `JDOODLE_CLIENT_ID`
- `JDOODLE_CLIENT_SECRET`

Make sure your Django settings file is configured to read environment variables (e.g., using `python-dotenv` or `os.environ`).

### ✅ Frontend (`frontend-React/viksitai/.env`)

Inside the `viksitai/` folder, create a `.env` file and add the following keys:

- `VITE_APP_GITHUB_TOKEN`
- `VITE_APP_FIREBASE_API_KEY`
- `VITE_APP_FIREBASE_AUTH_DOMAIN`
- `VITE_APP_FIREBASE_PROJECT_ID`
- `VITE_APP_FIREBASE_STORAGE_BUCKET`
- `VITE_APP_FIREBASE_MESSAGING_SENDER_ID`
- `VITE_APP_FIREBASE_APP_ID`
- `VITE_APP_FIREBASE_MEASUREMENT_ID`
- `VITE_APP_JDOODLE_CLIENT_ID`
- `VITE_APP_JDOODLE_CLIENT_SECRET`
- `VITE_APP_SARVAM_API_KEY`

These are used in the frontend for:
- Firebase integration
- GitHub and code execution API access
- AI interactions



## 🚀 Getting Started

### Backend (Django)

```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver

### Frontend (React)

cd frontend-React/viksitai
npm install
npm run dev
