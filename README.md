

```markdown
# Upwork Automation using n8n (Dockerized)

This project is a **production-ready, AI-driven automation workflow** built using **n8n**, designed to automatically fetch, score, and prioritize Upwork job listings related to **automation and AI workflows**.

---

## 🚀 Features

- ⏰ Scheduled execution every 8 hours  
- 🌐 Fetches Upwork jobs using **Apify API** (last 6 hours)  
- 🧠 Skill-based scoring using custom JavaScript logic  
- 🤖 AI-powered job relevance scoring (Gemini / OpenAI compatible)  
- 🎯 Pre-filters jobs by budget and experience level  
- 🚨 Email alerts for high-priority jobs  
- 📊 Stores qualified jobs in **Airtable**  
- 🧾 Centralized error handling and logging  
- 🐳 Fully Dockerized setup  

---

## 🧱 Tech Stack

- **n8n** (Self-hosted)
- **Docker & Docker Compose**
- **Apify**
- **Google Gemini / OpenAI**
- **Airtable**

---

## 📦 Project Structure

```

upwork-automation-n8n/
├── workflow/
│   └── Upwork-Automation-Enhanced.json
├── docker-compose.yml
├── .env.example
├── .gitignore
└── README.md

````

---

## ⚙️ Setup Instructions (Docker)

### 1. Clone the Repository
```bash
git clone https://github.com/Ayush-kr-007/upwork-automation-n8n.git
cd upwork-automation-n8n
````

### 2. Create Environment File

```bash
cp .env.example .env
```

### 3. Configure Environment Variables

```env
N8N_BASIC_AUTH_ACTIVE=true
N8N_BASIC_AUTH_USER=admin
N8N_BASIC_AUTH_PASSWORD=admin123

APIFY_API_TOKEN=your_apify_token
OPENAI_API_KEY=your_openai_or_gemini_key
AIRTABLE_API_KEY=your_airtable_key
```

### 4. Start n8n

```bash
docker compose up -d
```

### 5. Access n8n Dashboard

```
http://localhost:5678
```

---

## ▶️ Running the Workflow

1. Import the workflow JSON from the `workflow/` folder
2. Run once manually to validate execution
3. Enable the workflow for scheduled execution (every 8 hours)

---

## 📊 Airtable Output Fields

* Job Title
* Job Description
* Score
* Priority
* Reasoning

---

## 🚨 Error Handling

* Any workflow failure triggers the **Error Trigger** node
* Errors are logged into **Airtable** with execution details and timestamps

---

## 🎥 Demo Video

The demo video showcases:

* Workflow execution
* AI-based job scoring
* Airtable data population
* High-priority job email alerts

---

## ✅ Status

* ✅ Workflow runs end-to-end
* ✅ All assignment requirements completed
* ✅ Production-ready setup

---

## 👤 Author

**Ayush Kumar**

---

Paste → Save → `git commit` → `git push`

You’re **done**. 🫡

```

- or badges + screenshots section

Say the word.
```
