# Formspree MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/formspree)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/formspree-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/formspree-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage form submissions and automate data collection via Formspree — list entries, filter by date, and submit new data directly from your AI agent.

## Description
Connect your **Formspree** account to any AI agent to streamline your lead capture and form management workflows through natural conversation.

### What you can do

- **Submission Retrieval** — Fetch all entries for specific forms using their unique hash IDs to analyze leads or feedback.
- **Advanced Filtering** — Query submissions with pagination, date filters (`since`), and custom sort orders to find exactly what you need.
- **Direct Submission** — Programmatically submit data to forms including contact info, messages, and custom fields like company or phone.
- **Spam Management** — Optionally include or exclude flagged submissions in your queries to keep your data clean.

### How it works

1. Subscribe to this server
2. Enter your Formspree API Key
3. Start managing your form data from Claude, Cursor, or any MCP-compatible client

No more manual exporting of CSVs to check your latest leads. Your AI acts as a dedicated data analyst and form administrator.

### Who is this for?

- **Marketing Teams** — instantly retrieve latest campaign leads and filter by date without leaving the chat.
- **Developers** — test form submissions and verify data flow directly from the code editor.
- **Customer Support** — check recent form inquiries to respond to users faster and more efficiently.


## Available Tools
- **list_submissions**: Get submissions for a specific form
- **submit_form**: Does not require API key authentication.

Submit data to a form


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Formspree** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 submissions for form hashid 'mqkvpogq'."

**🤖 AI Agent:**
> I've retrieved the 5 most recent submissions for form 'mqkvpogq'. They include entries from 'Alice Smith' and 'Bob Jones' regarding 'Project Inquiry'. Would you like to see the full message for any of these?

---

**👤 You:**
> "Check for any new submissions for form 'xknpdyzd' since 2024-01-01."

**🤖 AI Agent:**
> Searching for submissions since January 1st... I found 3 new entries. One is a newsletter signup and two are contact requests. Shall I summarize the contact requests for you?

---

**👤 You:**
> "Submit a test entry to form 'mqkvpogq' with name 'Test User' and message 'Hello from MCP'."

**🤖 AI Agent:**
> Submitting data... The test entry was successfully sent to form 'mqkvpogq'. Formspree confirmed the submission was received.


## Installation & Usage

To install and use the **Formspree** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/formspree](https://vinkius.com/mcp/formspree)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
