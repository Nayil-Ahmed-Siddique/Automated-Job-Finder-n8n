# automated-job-finder-n8n

![Workflow Diagram](./WorkflowOverview.png)

🚀 Automated Job Finder – Email Alerts (n8n)

An end-to-end automation workflow built with n8n that aggregates software engineering job postings from multiple sources, filters them intelligently, scores job quality, and delivers curated job alerts via email.
This project demonstrates real-world automation design, not toy examples.

🔍 What This Project Does

Fetches job postings from multiple RSS job sources
Merges and normalizes incoming data
Filters jobs based on:
Software / engineering roles
Country or location criteria
Applies custom job quality scoring using JavaScript
Sends structured email alerts with relevant job links
Designed to scale by simply adding more RSS feeds

🧠 Why This Project Matters

This workflow demonstrates:
Practical automation design (not scripts)
Data ingestion from multiple sources
Conditional logic and branching
Custom business logic using JavaScript nodes
Clean separation of concerns
Production-ready thinking using schedulers and filters
Built to show how automation replaces manual job searching.

🧩 Workflow Architecture
High-level Flow
Schedule Trigger
   ├─ RSS Feed 1
   ├─ RSS Feed 2
   ├─ RSS Feed 3
        ↓
      Merge
        ↓
 Filter: Software Jobs
        ↓
 Filter: Country
        ↓
 Job Scoring (Code)
        ↓
 Quality Filter
        ↓
 Email Content Builder
        ↓
 Send Email
 
🖼 Workflow Diagram

![Workflow Diagram](./WorkflowOverview.png)

🛠 Tech Stack

n8n – workflow orchestration
RSS – job data ingestion
JavaScript (Code nodes) – scoring & filtering logic
Email node – automated notifications

📦 Repository Contents
.
├── workflow-diagram.png      # Visual workflow overview
├── workflow.json             # Exported n8n workflow
└── README.md                 # Project documentation

▶ How to Run This Workflow

Install or open n8n
Import the workflow.json file
Configure:
RSS feed URLs
Email credentials
Activate the workflow
Let the scheduler run automatically

🎯 Use Cases

Automated job discovery
Email alert systems
Content aggregation pipelines
Resume-ready automation projects

📌 Notes

This project is intentionally kept simple and extensible
New RSS feeds or filters can be added without redesign
Built as a portfolio-grade automation, not a demo

👤 Author

Nayil Ahmed Siddique
AI / Automation Engineer
(Project built to demonstrate real-world automation skills)
