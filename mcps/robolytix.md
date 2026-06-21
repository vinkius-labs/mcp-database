# Robolytix MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/robolytix)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/robolytix-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/robolytix-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Monitor robotic process automation performance with analytics that track bot execution times, success rates, and exceptions.

## Description
Connect your **Robolytix** account to any AI agent and take full control of your robotic process automation (RPA) analytics and performance orchestration through natural conversation. Robolytix provides a specialized platform for monitoring bot workflows and business process health, and this integration allows you to send sonar messages, track process runs, and manage automation metadata directly from your chat interface.

### What you can do

- **Process & Sonar Orchestration** — Trigger process 'sonars' programmatically to track starts, common steps, and end-of-process events across your automation stack.
- **Run Lifecycle Management** — Access and monitor individual process runs and retrieve detailed metadata to ensure your bots are performing optimally directly from the AI interface.
- **Performance & Error Intelligence** — Log process errors and retrieve real-time status updates via natural language to maintain high-quality automation uptime.
- **Process Discovery** — List and search through your configured robotic processes to find the correct identifiers for orchestration.
- **Operational Monitoring** — Track system activity and manage sonar metadata using simple AI commands to ensure your RPA analytics are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Robolytix API Key from your account settings
3. Start managing your RPA performance from Claude, Cursor, or any MCP-compatible client

No more manual status checking or bot log hunting. Your AI acts as a dedicated RPA operations manager or performance analyst.

### Who is this for?

- **RPA Developers & DevOps** — quickly retrieve process statuses and monitor bot health without switching dashboards.
- **Automation Managers** — automate the logging of process milestones and track run durations via natural conversation.
- **Business Analysts** — streamline the retrieval of process metadata and monitor organizational automation health directly within the chat.


## Available Tools
- **get_process**: Get details for a specific process
- **get_run_messages**: Get all messages from a process run
- **get_run**: Get details for a specific process run
- **get_stats**: Get overall automation statistics
- **list_rpa_processes**: List all RPA processes
- **list_runs**: List all process runs
- **sonar_checkpoint**: Send a "common" sonar message
- **sonar_end**: Send an "end" sonar message
- **sonar_error**: Send an "error" sonar message
- **sonar_start**: Send a "start" sonar message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Robolytix** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Log the start of process 'p-123' with run ID 'r-999'."

**🤖 AI Agent:**
> Sonar start message sent! Process 'p-123' is now being tracked under run 'r-999' in Robolytix. Would you like to log a common step now?

---

**👤 You:**
> "Show me all RPA process runs from today with their success rates and execution times."

**🤖 AI Agent:**
> 34 process runs today across 8 automated processes. Success: 31 (91.2%). Failed: 3 (invoice processing errors). "Order Processing" ran 12 times (avg 2.3 min, 100% success). "Invoice Generation" ran 8 times (avg 1.8 min, 75% success, 2 failures due to template mismatch). "Data Sync" ran 6 times (avg 4.5 min, 100% success). "Email Classification" ran 5 times (avg 0.8 min, 100% success). Total automation time saved: 4.2 hours. Cost savings: $840.

---

**👤 You:**
> "Get the detailed message log for the last failed invoice processing run."

**🤖 AI Agent:**
> Run ID: run_8923 (Invoice Generation, failed at 10:47 AM). 12 messages in log. Start: "Process initiated, 45 invoices queued". Steps 1-8: successful (customer lookup, line item calculation, tax computation). Step 9 ERROR: "Template 'INV-2024-v3' not found. Expected path: /templates/invoices/". Step 10: "Attempting fallback template 'INV-2024-v2'". Step 11 ERROR: "Fallback failed - missing required field 'tax_region'". End: "Process terminated with error code E-TPL-404". Recommendation: update template path in config.


## Installation & Usage

To install and use the **Robolytix** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/robolytix](https://vinkius.com/mcp/robolytix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
