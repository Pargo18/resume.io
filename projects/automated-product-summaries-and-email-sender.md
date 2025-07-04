---
layout: single
title: "Automated product summaries generation and email sending"
permalink: /projects/summaries-email/
---

# 📧 Review Automator – GPT-Based Review Summarizer with Email Automation & Web Scraping

**Review Automator** is a complete Python automation system that scrapes product reviews from forums, generates intelligent summaries using GPT, and delivers structured, readable reports via automated email. This tool is built for product teams, brand managers, or operations staff who need regular insights from live user feedback — without spending hours reading raw comments.

---

## 🧠 What It Does

Customer feedback from forums and community threads often contains valuable insights — but it’s buried in messy, unstructured conversations. This tool automates the process by:

- **Scraping reviews or user discussions** from a forum or message board
- **Cleaning and formatting** the extracted text
- **Generating summaries** using GPT (OpenAI integration)
- **Sending automated email reports** to stakeholders

No more copy-pasting forum threads or manually interpreting customer pain points. This automation handles the entire loop — from data collection to delivery.

---

## 🔧 Features

### ✅ Web Scraping
- Extracts user reviews or discussion posts from a target forum (e.g., product-specific thread)
- Can be configured for pagination, specific user filters, or topic keywords
- Uses `requests`, `BeautifulSoup`, and optional headless browsing for dynamic sites

### 🤖 GPT Summarization
- Integrates with OpenAI’s GPT models (e.g., `gpt-3.5-turbo`, `gpt-4`)
- Parses raw user-generated content into:
  - Concise summaries
  - Bullet-point pros and cons
  - Highlighted recurring themes or complaints
- Configurable prompt templates to adjust summarization tone or length

### ✉️ Email Automation
- Sends formatted summaries via email on demand or on a schedule
- HTML and plain text email formats supported
- Multiple recipients, CC/BCC, dynamic subject lines
- Configurable SMTP (Gmail, Outlook, etc.)

---

## 📊 Typical Output

An email per scraped thread or product, containing:

- 🧵 Source title and scrape time
- 🧠 GPT-generated summary of the user feedback
- ✅ Most mentioned positive points
- ⚠️ Common user frustrations or issues
- 📎 Attached summary as `.txt` or `.xlsx` file (optional)

---

## 🚀 Example Use Case

> You’re tracking community feedback on a tech product.  
> Instead of checking forums daily and summarizing posts manually, you run Review Automator. It:
> - Scrapes the relevant discussion thread
> - Cleans and parses the user comments
> - Sends a structured summary email to your team every morning  
> 
> → You never miss trends in customer feedback again.

---

## ⚙️ Tech Stack

- **Python 3.10+**
- `requests`, `BeautifulSoup` – web scraping
- `pandas`, `openpyxl` – data structuring & Excel export
- `openai` – GPT integration for summaries
- `smtplib`, `email`, `jinja2` – email automation
- `dotenv` – for secure environment config

> For part of the code, visit the [GitHub repository](https://github.com/Pargo18/Email-sender-automation)