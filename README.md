# 🤖 Groq AI Chatbot — Backend Version

Users can chat without entering any API key!

## Project Structure
```
chatbot/
├── app.py            ← Flask backend (hides your API key)
├── requirements.txt  ← Python dependencies
├── Procfile          ← For Render deployment
└── static/
    └── index.html    ← Frontend UI
```

## Run Locally

1. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

2. Set your Groq API key in app.py (line 9):
   ```python
   GROQ_API_KEY = "your_key_here"
   ```

3. Run the server:
   ```
   python app.py
   ```

4. Open browser: http://localhost:5000

---

## 🚀 Host for FREE on Render.com

1. Upload this folder to a GitHub repo
2. Go to https://render.com → Sign up free
3. Click "New" → "Web Service"
4. Connect your GitHub repo
5. Set these settings:
   - Build Command: `pip install -r requirements.txt`
   - Start Command:  `gunicorn app:app`
6. Add Environment Variable:
   - Key:   `GROQ_API_KEY`
   - Value: `your_groq_api_key_here`
7. Click "Deploy" — you get a free public URL!

Your chatbot will be live at: https://your-app-name.onrender.com
