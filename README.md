
# AI Study Buddy — v1.0 (Minimal)

A simple Streamlit chat app that helps students learn **any subject in English**.
It mirrors the user's tone (casual/formal) and explains concepts step-by-step.

## Features (v1.0 Minimal)
- Clean chat UI (mobile-friendly)
- One friendly intro message
- English-only replies
- Adaptive style (via system prompt)
- Footer credit: “Created by HarshVardhan”

## Local Setup
1. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
2. **Set your OpenAI API key**
   ```bash
   export OPENAI_API_KEY="sk-..."
   # optional: choose a model
   export OPENAI_MODEL="gpt-4o-mini"
   ```
3. **Run the app**
   ```bash
   streamlit run app.py
   ```

## Deploy on Streamlit Community Cloud
1. Push these files to a GitHub repo (e.g., `ai-study-buddy`).
2. Go to https://streamlit.io/cloud → **New app** → connect your GitHub repo.
3. In **App settings → Secrets**, add:
   ```
   OPENAI_API_KEY = "sk-..."
   OPENAI_MODEL = "gpt-4o-mini"
   ```
4. Click **Deploy**. Your app link will be generated.

## Notes
- You can swap `OPENAI_MODEL` to any compatible model in your account.
- For streaming tokens, you can adapt to OpenAI's streaming guide later.
- This v1 keeps things simple; you can add random intros, typing animation,
  and level selection in future versions.
