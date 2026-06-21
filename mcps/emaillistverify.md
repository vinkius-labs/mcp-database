# EmailListVerify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emaillistverify)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/emaillistverify-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/emaillistverify-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to verify email deliverability, manage bulk verification jobs, and track credits via the EmailListVerify API.

## Description
Integrate **EmailListVerify**, the powerful bulk email verification platform, directly into your AI workflow. Verify individual email addresses for deliverability, manage large-scale verification jobs and files, monitor real-time processing statuses, and oversee your verification credits using natural language.

### What you can do

- **Single Verification** — Instantly verify a single email address, resolving MX records, SMTP connection checks, and identifying disposable emails.
- **Bulk Job Oversight** — List and retrieve detailed status and results for all your uploaded email verification files.
- **Credit Management** — Access real-time credit balance information and remaining organizational quotas for email verification.
- **Verification Auditing** — Retrieve high-level summaries of processing activity, success rates, and identified invalid email patterns instantly.

### How it works

1. Connect the EmailListVerify integration to your AI assistant.
2. Authorize using your EmailListVerify API Key (found in your account settings).
3. Orchestrate your email list hygiene and deliverability analysis through intuitive conversation.

### Who is this for?

- **Email Marketers** — Quickly check list cleaning status and verify individual emails on the go.
- **CRM Managers** — Research email quality and identify invalid addresses via chat during data entry.
- **Operations Teams** — Monitor credit balances and organizational verification metadata instantly.


## Available Tools
- **get_emaillistverify_metadata**: Retrieve metadata and settings for your EmailListVerify account
- **get_remaining_credits**: Retrieve the number of remaining verification credits in your account
- **get_verification_job_status**: invalid addresses.

Get the current status and results summary for a specific bulk verification job
- **quick_verification_health_audit**: Retrieve a high-level summary of verification activity and success rates
- **list_successfully_processed_files**: Identify bulk verification jobs that have finished processing
- **list_in_progress_verification_jobs**: Identify bulk verification jobs that are currently in the processing queue
- **list_latest_verification_jobs**: Identify the most recently uploaded email verification files
- **list_verification_jobs**: List all bulk email verification files/jobs in your account
- **verify_single_email**: Verify a single email address for deliverability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EmailListVerify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify if 'test@example.com' is a valid email address."

**🤖 AI Agent:**
> I've verified 'test@example.com'. The status is 'ok' (Valid). It has valid MX records and the SMTP check passed. Should I check if it's a disposable email address?

---

**👤 You:**
> "Show me the status of our last 5 verification jobs."

**🤖 AI Agent:**
> I've retrieved your recent jobs. 4 are 'Finished' and 1 is 'In Progress' (65% complete). Finished lists include 'Newsletter_Clean_Q1.csv' and 'Leads_Export.txt'. Would you like the results summary for Newsletter_Clean_Q1?

---

**👤 You:**
> "How many verification credits do I have left?"

**🤖 AI Agent:**
> You currently have 12,450 verification credits remaining in your account. Your last purchase was for 20,000 credits on March 1st. Should I list any recently processed files that used these credits?


## Installation & Usage

To install and use the **EmailListVerify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emaillistverify](https://vinkius.com/mcp/emaillistverify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
