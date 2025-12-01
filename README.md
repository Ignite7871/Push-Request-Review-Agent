🚀 AI Pull Request Reviewer Agent

An automated LLM-powered code review assistant that analyzes GitHub Pull Requests, providing intelligent suggestions and quality checks using Google Gemini AI, Flask, and GitHub Webhooks.

This system reduces repetitive review effort for developers, ensures consistency in coding standards, and speeds up the overall software delivery process.

✨ Key Features

🔍 Automated Code Review
Uses Gemini AI to generate meaningful feedback on code logic, structure, documentation, and best practices.

🧠 LLM-Based Reasoning
Improves code quality by detecting potential bugs, missing validations, and optimization opportunities.

🔁 CI/CD Integration via GitHub Webhooks
Triggers automatically when a Pull Request is opened, updated, or synchronized.

📈 Productivity Boost
Reduces manual code review time by ~45% by filtering trivial issues and highlighting critical improvements.

🏗️ System Architecture
flowchart LR
    A[Developer Creates/Updates PR] --> B[GitHub Webhook Trigger]
    B --> C[Flask Backend]
    C --> D[Gemini AI Code Analysis]
    D --> C
    C --> E[GitHub API Comments on PR]

🔧 Tech Stack
Component	Technology
Backend Framework	Flask
Language	Python
AI Model	Google Gemini API
DevOps & Integration	GitHub REST API + Webhooks
Deployment	Local / Cloud Support
📦 Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/<your-username>/pr-review-agent.git
cd pr-review-agent

2️⃣ Install dependencies
pip install -r requirements.txt

3️⃣ Add environment variables

Create a .env file:

GEMINI_API_KEY=your_google_api_key
GITHUB_TOKEN=your_personal_access_token

4️⃣ Run the server
python app.py

5️⃣ Configure GitHub Webhook

Go to GitHub Repo → Settings → Webhooks

Add payload URL:
http://<your-server-url>/webhook

Select event: Pull Request

Set content type: application/json

⚙️ How It Works
Action	Response
New/Updated Pull Request	Gemini evaluates changes and comments with suggestions
Detected security/logic issue	Highlights improvements directly on PR
Code quality analysis	Rates clarity, efficiency, best practices adherence
