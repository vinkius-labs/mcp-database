# OneTrust MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/onetrust)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/onetrust-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/onetrust-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage privacy requests, assessments, vendors, consent, and incidents via OneTrust — automate GDPR, CCPA, and data governance from any AI agent.

## Description
Connect your **OneTrust** account to any AI agent and manage privacy compliance, vendor risks, and data governance through natural conversation.

### What you can do

- **Data Subject Requests** — List, create, and track DSARs (GDPR/CCPA access, deletion, opt-out requests)
- **Privacy Assessments** — Browse PIAs, DPIAs, and Transfer Impact Assessments with risk scores
- **Data Inventory** — View the data map: which systems process personal data, for what purpose, and under which legal basis
- **Vendor Risk** — Manage third-party vendors with security questionnaires and risk ratings
- **Consent Management** — Review consent purposes and cookie categories
- **Incident Management** — Track privacy and security incidents with severity and regulatory notification status
- **Risk Register** — View identified risks with impact, likelihood, and treatment plans

### How it works

1. Subscribe and enter your OneTrust API token (from **Admin Console → Integration → API Access**)
2. Your AI agent connects to your OneTrust instance
3. Ask questions like "show me open DSARs" or "which vendors have overdue assessments?"

### Who is this for?

- **Data Protection Officers** — Track DSARs, assessments, and compliance posture without opening OneTrust
- **Privacy Teams** — Manage data inventory, consent, and vendor risks through conversation
- **Security & Compliance** — Monitor incidents, risks, and regulatory deadlines from anywhere


## Available Tools
- **onetrust_create_dsar**: Request types: ACCESS (subject wants their data), DELETION (right to be forgotten), RECTIFICATION (correct inaccurate data), PORTABILITY (data export), OPT_OUT (stop selling/sharing). The request enters the fulfillment workflow with regulatory deadlines automatically calculated (e.g., 30 days for GDPR).

Create a new data subject access request in OneTrust — register a GDPR/CCPA privacy request on behalf of an individual
- **onetrust_get_assessment**: Use for assessment review, audit evidence, or understanding the privacy risk landscape of a specific project or data processing activity.

Get full details of a privacy impact assessment — questions, responses, risk findings, and recommendations from the review process
- **onetrust_get_dsar**: 15/17/20, CCPA §1798.100), processing steps completed, data sources discovered, assigned handler, deadline, and audit trail. Use for detailed DSAR investigation, compliance verification, or reporting.

Get complete details of a specific data subject request — subject information, request history, fulfillment steps, and regulatory context
- **onetrust_list_assessments**: Each shows: assessment name, type, risk score, status (Draft/In Review/Approved/Rejected), assigned owner, and completion date. Use for GDPR Art. 35 compliance, risk oversight, or assessment pipeline review.

List privacy impact assessments (PIAs/DPIAs) in OneTrust — Data Protection Impact Assessments with risk scores and approval status
- **onetrust_list_assets**: Each asset includes: name, type, data categories processed, processing purposes, legal basis, data subjects affected, retention periods, and risk classification. Essential for GDPR Art. 30 compliance. Use when the user asks about "what systems process personal data?" or needs the data map.

List data inventory assets in OneTrust — applications, databases, systems, and third-party services with data classification and processing purposes
- **onetrust_list_consent_purposes**: Each purpose includes: name, description, category (Strictly Necessary/Performance/Functional/Marketing), associated cookies/trackers, and default consent state. Purposes are the building blocks of your cookie banners and preference centers. Use for consent configuration review or privacy banner auditing.

List consent purposes configured in OneTrust consent management — cookie categories, marketing preferences, and data collection purposes
- **onetrust_list_dsars**: Each DSAR includes: subject name, email, request type (Access/Deletion/Rectification/Portability/Opt-Out), current status (Open/In Progress/Completed/Overdue), assigned handler, submission date, and regulatory deadline. Use when the user asks about pending privacy requests, DSAR compliance, or deadline tracking.

List data subject access requests (DSARs) in OneTrust — GDPR, CCPA, and privacy rights requests from individuals with status and deadlines
- **onetrust_list_incidents**: Each incident includes: title, severity (Critical/High/Medium/Low), status (Open/Under Investigation/Resolved/Closed), type (Data Breach/Near Miss/Complaint), affected data subjects count, regulatory notification status, and assigned investigator. Use for breach response management, regulatory reporting requirements, or incident trend analysis.

List security and privacy incidents in OneTrust incident management — breaches, near-misses, and reports with severity and regulatory notification status
- **onetrust_list_risks**: Each risk includes: title, description, category, impact level, likelihood score, calculated risk rating, treatment plan (Accept/Mitigate/Transfer/Avoid), associated controls, and assigned owner. Use for enterprise risk management reporting, board-level risk summaries, or identifying areas that need attention.

List privacy and security risks from OneTrust risk register — identified risks with impact, likelihood, risk score, and treatment plans
- **onetrust_list_vendors**: Each vendor shows: name, risk score, assessment status (questionnaire sent/completed/overdue), data categories shared, contractual safeguards (DPA signed/pending), and last review date. Use for vendor due diligence, subprocessor management, or GDPR Art. 28 compliance verification.

List third-party vendors in OneTrust vendor risk management — data processors, subprocessors, and partners with security/privacy risk ratings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OneTrust** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many open data subject requests do we have?"

**🤖 AI Agent:**
> You have **7 open DSARs**:

🔴 **2 overdue** — Both are deletion requests (GDPR Art. 17) past the 30-day deadline
🟡 **3 in progress** — 1 access request, 2 portability requests (due in 12, 18, 22 days)
🟢 **2 new** — Submitted today, auto-routed to the Privacy Team

The 2 overdue requests need immediate attention — shall I show the details?

---

**👤 You:**
> "Which vendors have overdue security assessments?"

**🤖 AI Agent:**
> There are currently 4 vendors with overdue security assessments:
1. CloudHost Inc. (High Risk) - Overdue by 15 days
2. DataFlow Analytics (Medium Risk) - Overdue by 8 days
3. MailSender Corp (Low Risk) - Overdue by 3 days
4. CDN Partners (Medium Risk) - Overdue by 1 day
Would you like me to trigger automated reminders for these vendors?

---

**👤 You:**
> "Show the data map for our CRM system."

**🤖 AI Agent:**
> Here is the data map for the CRM System:
- **Personal Data Processed:** Names, email addresses, phone numbers, purchase history.
- **Purpose:** Customer relationship management, direct marketing.
- **Legal Basis:** Legitimate interest (CRM), Consent (Direct Marketing).
- **Retention Period:** 5 years after last contact.
The CRM system is fully compliant with current policies.


## Installation & Usage

To install and use the **OneTrust** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onetrust](https://vinkius.com/mcp/onetrust)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
