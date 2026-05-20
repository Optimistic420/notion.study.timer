# notion.study.timer
The one solution notion timer html version for embedding

# JEE Study Tracker with Automated Notion Sync

A sleek, lightweight, minimalist HTML/JavaScript study timer designed to track intensive preparation sessions. This tracker features a local analytics dashboard and is fully integrated with a cloud-based Notion database via custom webhooks for permanent data storage.

## 🚀 Features

- **Dynamic Timer:** Built-in validation that automatically discards accidental triggers (sessions under 5 seconds).
- **Custom Categorization:** Tracks study sessions across core subjects (Physics, Chemistry, Math) with custom text memos/notes.
- **Local Analytics Dashboard:** Displays current and historical session metrics directly in the browser using `localStorage`.
- **Cloud Database Sync:** Automatically streams log data across the web to a designated Notion workspace workspace in real-time.
- **Independent History Purging:** Includes a local reset utility that wipes browser-cached history without affecting or modifying archived cloud rows.

## 🛠️ Architecture & Workflow

The system operates via a continuous three-tiered data pipeline:

1. **Frontend (Client Side):** The customized HTML structure handles the timer engine and captures session inputs (`subject`, `duration`, `notes`, and real-time `start/end` clock timestamps).
2. **Middleware API (Make.com):** A headless server endpoint listens for incoming network `POST` requests payload transmissions, captures the JSON data stream, and standardizes field configurations.
3. **Backend Database (Notion):** A structured data table receiving real-time logs, utilizing dynamic formulas to parse raw data (e.g., converting runtime minutes into decimal hour increments).

## 💻 Tech Stack

- **Frontend:** Semantic HTML5, CSS3 (Serif Typography Layout), JavaScript (ES6+ Web Fetch API)
- **Automation / Integration:** Make.com Webhook Integration Engine
- **Database System:** Notion API / Relational Database Workspace

---
*Created as part of an automated workflow setup for tracking core academic milestones.*


Delployed website url : [Timer](https://optimistic420.github.io/notion.study.timer/study_timer.html)
