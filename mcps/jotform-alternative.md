# Jotform MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jotform-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jotform-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jotform-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Build powerful online forms with drag-and-drop ease, collect payments, gather signatures, and process submissions automatically.

## Description
Connect your **Jotform** account to any AI agent and manage forms and submissions through natural conversation.

### What you can do

- **Form Browsing** — List all forms with submission counts and status
- **Submission Management** — Read form responses, filter by date, and inspect individual entries
- **Form Properties** — Inspect form fields, settings, and configuration
- **Report Access** — View form reports and analytics dashboards
- **User Management** — Access account details and usage statistics
- **Folder Organization** — Browse form folders for organized management

### How it works

1. Subscribe to this server
2. Enter your Jotform API Key from account settings
3. Start managing forms from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing** — track form conversion rates and analyze submission data
- **Operations** — manage intake forms and review responses
- **Developers** — integrate form data into AI-powered workflows


## Available Tools
- **list_submissions_for_form**: List responses for a specific form
- **get_form_details**: Get metadata for a specific form
- **list_account_history**: List recent account activities
- **get_form_questions**: Get questions defined in a form
- **get_submission_details**: Get full data for a single submission
- **get_api_usage**: Check API and plan usage
- **list_form_folders**: List your organizational folders
- **list_forms**: List all forms in your account
- **list_form_reports**: List generated reports
- **list_all_submissions**: List recent submissions across all forms


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jotform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all forms with submission counts and the latest responses from the contact form."

**🤖 AI Agent:**
> Forms: 12 total. 'Contact Us' (456 submissions), 'Job Application' (89), 'Event Registration' (234), 'Customer Feedback' (178), 8 others. Latest 'Contact Us' responses: 1) Ana Costa — 'Interested in enterprise pricing' (today, 10:15 AM). 2) Mike Torres — 'Technical support request' (today, 9:30 AM). 3) Lisa Park — 'Partnership inquiry' (yesterday). Would you like to view analytics or inspect form fields?

---

**👤 You:**
> "Show the analytics report for the Event Registration form and account usage."

**🤖 AI Agent:**
> Event Registration analytics: 234 submissions total. This month: 45. Conversion rate: 68% (visitors who complete). Avg completion time: 3.2 min. Top source: Direct (42%), Social (28%), Email (18%). Peak day: Wednesday. Account: 12 forms, 957 total submissions, 2.1 GB storage used. Plan: Bronze (10,000 submissions/mo).

---

**👤 You:**
> "Inspect the fields of the Job Application form and list submissions from this week."

**🤖 AI Agent:**
> Job Application fields: 10. Full Name (text, required), Email (email, required), Phone (phone), Resume (file upload, PDF only, max 10MB), Cover Letter (textarea), Position (dropdown: Engineer, Designer, PM, Sales), Experience (number), LinkedIn (URL), Start Date (date), Referral Source (radio). This week: 8 submissions. Engineers: 4, Designers: 2, PMs: 1, Sales: 1. 6 have resumes attached.


## Installation & Usage

To install and use the **Jotform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jotform-alternative](https://vinkius.com/mcp/jotform-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
