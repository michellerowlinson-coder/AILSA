# Ailsa — AI Life Coach
## Vercel Deployment Guide

---

### FOLDER STRUCTURE
```
ailsa-vercel/
├── index.html        ← Ailsa's chat page
├── ailsa.jpg         ← Ailsa's photo
├── vercel.json       ← Vercel config
├── README.md         ← This guide
└── api/
    └── chat.js       ← Secure Gemini API function
```

---

### STEP 1 — Deploy to Vercel
1. Go to https://vercel.com and log in
2. Click "Add New" → "Project"
3. Look for "Deploy without a Git repository" or drag and drop option
4. Upload or drag the entire "ailsa-vercel" folder
5. Click Deploy — you'll get a live URL in about 30 seconds

---

### STEP 2 — Add your Gemini API Key
1. In Vercel go to your project → "Settings" → "Environment Variables"
2. Click "Add"
3. Name:  GEMINI_API_KEY
   Value: AIza... (your Google Gemini API key)
4. Click Save
5. Go to "Deployments" → click the three dots on the latest deploy → "Redeploy"

---

### STEP 3 — Embed in Wix
1. Copy your Vercel URL e.g. https://ailsa.vercel.app
2. In Wix Editor: Add (+) → Embed & Social → Embed a Widget
3. Paste this code:
<iframe src="YOUR_VERCEL_URL" width="100%" height="500" frameborder="0" style="border-radius:20px; border:none;"></iframe>

---

### TROUBLESHOOTING
- Ailsa not responding? Check GEMINI_API_KEY in Vercel environment variables
- Redeploy after adding the key
- Check the Functions log in Vercel for error details
