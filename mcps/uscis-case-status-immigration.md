# USCIS Case Status (Immigration) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uscis-case-status-immigration)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/uscis-case-status-immigration-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/uscis-case-status-immigration-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Track USCIS immigration case statuses and processing history directly from your AI agent using receipt numbers.

## Description
Connect to the official USCIS developer portal to monitor immigration applications. This server allows your AI agent to fetch real-time updates on case statuses, processing history, and current milestones for any valid 13-character receipt number.

### What you can do

- **Real-time Status** — Get the current standing of any USCIS application (e.g., 'Case Was Approved', 'Request for Evidence Sent')
- **Historical Tracking** — Retrieve the full chronological history of actions taken on a specific case
- **Multi-Case Monitoring** — Ask your agent to check multiple receipt numbers in sequence to provide a summary of your entire portfolio
- **Milestone Analysis** — Understand exactly where an application sits in the processing pipeline without logging into the USCIS website

### How it works

1. Subscribe to this server
2. Enter your USCIS Developer Client ID, Secret, and Environment
3. Provide a 13-character receipt number (e.g., EAC, LIN, MSC, SRC, WAC, IOE)

### Who is this for?

- **Immigration Attorneys** — quickly check status updates for multiple clients directly from a chat interface or document editor
- **Applicants** — stay informed about your personal Green Card, Visa, or Citizenship application progress via natural language
- **HR & Global Mobility Teams** — monitor employee sponsorship cases and filing histories efficiently


## Available Tools
- **get_case_status**: Get USCIS case status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **USCIS Case Status (Immigration)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status of USCIS case EAC9999103402."

**🤖 AI Agent:**
> I've retrieved the status for EAC9999103402. It is currently 'Case Was Approved' as of October 12, 2023.

---

**👤 You:**
> "What is the history for case number LIN2190345678?"

**🤖 AI Agent:**
> The history for LIN2190345678 shows 3 major events: 1. Case Received (Jan 5), 2. Biometrics Appointment (Feb 10), and 3. Case is Being Actively Reviewed (Feb 12).

---

**👤 You:**
> "Give me the latest update on my immigration application MSC2290123456."

**🤖 AI Agent:**
> The latest update for MSC2290123456 is 'Request for Additional Evidence Was Sent' on March 15, 2024. You should expect a notice in the mail.


## Installation & Usage

To install and use the **USCIS Case Status (Immigration)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uscis-case-status-immigration](https://vinkius.com/mcp/uscis-case-status-immigration)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
