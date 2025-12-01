Push Request Reviewer Agent

Tools used: Flask, Python, Google Gemini API, GitHub REST API

Installation & Setup
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
