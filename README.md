🧠 Activity Tracker
This Python-based desktop activity tracker helps you log and analyze your app usage, browser activity, and productivity trends in a structured and insightful way.

🚀 Features
Tracks foreground application usage with timestamps

Classifies activities by categories (e.g., Work, Leisure, Communication)

Detects idle time

Monitors website activity via browser titles (e.g., YouTube, Gmail, Google Docs)

Generates CSV reports for analysis

Scoring system for productive vs unproductive time

Optional integration with Asana and Slack APIs

Designed for privacy – all logs stay local unless exported manually

📁 Project Structure
pgsql
Copy
Edit
activity-tracker/  
├── main.py                → Main tracking script  
├── activity_logger.py     → Logs and classifies activity  
├── idle_detector.py       → Detects periods of inactivity  
├── utils.py               → Helper functions  
├── config.json            → Customizable category mappings  
├── logs/                  → Stored CSV files  
└── README.md              → You're here!  
🛠️ Setup
Prerequisites
Python 3.8+

Required packages:

psutil

pyobjc-framework-Quartz (for macOS)

pynput

(Others as needed in requirements.txt)

Installation
Clone the repo:

bash
Copy
Edit
git clone https://github.com/yourusername/activity-tracker.git  
cd activity-tracker
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the tracker:

bash
Copy
Edit
python3 main.py
⚙️ Configuration
Customize:

Categories and keywords in config.json

Idle threshold (e.g., 300 seconds)

Productivity scoring system

📊 Output
Tracker generates .csv logs in the logs/ folder, including:

App name

Start and end time

Duration

Category

Website title (if detected)

Productivity score

Use the logs for time reviews or visualizations in Notion, Excel, or BI tools.

🔌 Optional Integrations
Asana: Map time blocks to tasks and subtasks

Slack: Analyze communication patterns and sentiment

📅 Coming Soon
Mac menu bar version

Notion database sync

Web dashboard with trend graphs

Timeline session replay

🙏 Acknowledgments
Built by Luke Wester to boost productivity, analyze behavior, and gamify deep work.

📝 License
MIT License. See LICENSE for details.

