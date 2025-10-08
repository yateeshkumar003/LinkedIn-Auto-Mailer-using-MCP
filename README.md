# 🚀 LinkedIn Auto-Mailer using MCP

## 📘 Overview

The **LinkedIn Auto-Mailer** is an automation tool that extracts LinkedIn profile data and automatically sends the extracted information to a predefined email address.  
This project leverages the power of **MCP (Model Context Protocol)** inside **Cursor IDE** to build a seamless, efficient, and secure workflow for automating LinkedIn data collection and email delivery.

By integrating data extraction, formatting, and email APIs, this tool helps recruiters, marketers, or data analysts automate their daily LinkedIn outreach or reporting tasks without manual intervention.

---

## 🧠 Key Features

✅ **Automated LinkedIn Data Extraction**  
Fetches user profile details such as name, headline, experience, education, and skills (depending on privacy permissions).

✅ **MCP-Based Workflow Automation**  
Uses **MCP (Model Context Protocol)** to create structured, contextual workflows that enable communication between data extraction, formatting, and email modules.

✅ **Email Auto-Sender**  
Automatically formats and sends the extracted LinkedIn profile data to a predefined email address using secure **Email APIs** (e.g., Gmail API, SendGrid, or SMTP).

✅ **Cursor IDE Integration**  
Fully developed and executed inside **Cursor IDE**, which supports AI-assisted MCP automation — allowing seamless debugging, context management, and testing of workflows.

✅ **Secure & Scalable**  
Implements authentication and token-based access to LinkedIn data and uses environment variables to store API keys securely.

---
## 🏗️ Architecture / Workflow

    ┌─────────────────────────┐
    │   LinkedIn Profile URL  │
    └────────────┬────────────┘
                 │
                 ▼
    ┌─────────────────────────┐
    │ Data Extraction (MCP)   │
    │ - Fetches profile info  │
    └────────────┬────────────┘
                 │
                 ▼
    ┌─────────────────────────┐
    │ Data Formatter (JS)     │
    │ - Cleans and structures │
    │   data for email body   │
    └────────────┬────────────┘
                 │
                 ▼
    ┌─────────────────────────┐
    │ Email Sender (API)      │
    │ - Sends to predefined   │
    │   recipient securely    │
    └─────────────────────────┘

---

## ⚙️ Tech Stack

| Component | Technology Used |
|------------|-----------------|
| **Automation Engine** | MCP (Model Context Protocol) |
| **Development Environment** | Cursor IDE |
| **Programming Language** | JavaScript |
| **Email Delivery** | Email API (Gmail / SMTP / SendGrid) |
| **Data Handling** | JSON-based structured data |
| **Security** | Environment variables for API keys |

---

## 💻 Installation & Setup

### Prerequisites
- Cursor IDE (with MCP enabled)
- Node.js installed (v18+ recommended)
- API keys for your email service provider (e.g., Gmail API or SendGrid)
- (Optional) LinkedIn API access token for large-scale profile fetching

### Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/linkedin-auto-mailer.git
   cd linkedin-auto-mailer
2. **Install dependencies:**
   ```bash
   npm install

3. Configure environment variables:
   Create a .env file in the root directory:
```bash
EMAIL_API_KEY=your_email_api_key
RECEIVER_EMAIL=example@domain.com
LINKEDIN_COOKIE=your_linkedin_session_cookie


4. Run the MCP automation workflow:
```bash
npm run mcp-start


5. Trigger the auto-mailer:
   Provide the LinkedIn URL inside Cursor IDE prompt or command line:
```bash
node sendProfile.js "https://www.linkedin.com/in/username/"

**Example Output**

Email Subject:

LinkedIn Profile Data - Dakoju Yateesh

**Email Body**
Name: John Doe
Headline: Software Engineer at Microsoft
Experience:
  - SDE II, Microsoft (2021–Present)
  - Software Developer, Infosys (2019–2021)
Education: B.Tech in Computer Science, NIT Trichy
Skills: JavaScript, React, AWS, DevOps


**Author**

Developed by: Dakoju Yateesh (Nxtwave Project)
Role: Developer 
Tools: MCP, Cursor IDE, JavaScript, Email API
