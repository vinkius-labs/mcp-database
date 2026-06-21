# Five9 QM MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/five9-qm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/five9-qm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/five9-qm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage agent evaluations, review recorded interactions, and track quality metrics via AI agents with Five9 QM.

## Description
Connect your **Five9 Quality Management (QM)** account to any AI agent and automate your quality assurance workflows through the Model Context Protocol (MCP). Five9 QM (formerly Virtual Observer) is a powerful tool for monitoring and scoring agent performance across voice and digital channels. Now, you can manage evaluations and review interactions directly through natural conversation.

### What you can do

- **Evaluation Management** — List all completed evaluations, fetch detailed scores and feedback, and submit new evaluations instantly.
- **Interaction Review** — Access recorded voice and digital interactions available for quality review and retrieve their full metadata.
- **Recording Retrieval** — Generate temporary, secure links to audio recordings for direct playback and analysis.
- **Form Inspection** — List all active quality evaluation forms and fetch their specific question and scoring structures.
- **Calibration Monitoring** — Track active and completed calibration sessions to ensure scoring consistency across your QA team.
- **Agent & User Discovery** — List agents available for evaluation and manage QM system users for better team context.
- **High-level Reporting** — Fetch QM summary metrics to understand organization-wide quality trends and performance.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Five9 VCC Username and Password (ensure QM permissions are enabled)
3. Start managing your quality assurance data from Claude, Cursor, or any MCP client

### Who is this for?

- **Quality Assurance (QA) Analysts** — quickly pull interaction details or submit evaluations without leaving your primary workspace.
- **Contact Center Managers** — get a real-time overview of quality scores and calibration progress through simple AI commands.
- **Team Leads** — review specific agent recordings and feedback to facilitate more effective coaching sessions.


## Available Tools
- **create_evaluation**: Submit a new evaluation
- **get_evaluation_form**: Get form structure
- **get_evaluation**: Get evaluation details
- **get_qm_interaction**: Get interaction metadata
- **get_qm_summary**: Get QM summary report
- **get_recording_link**: Get audio recording link
- **list_calibrations**: List calibration sessions
- **list_evaluation_forms**: List evaluation forms
- **list_evaluations**: List agent evaluations
- **list_qm_agents**: List evaluatable agents
- **list_qm_interactions**: List recorded interactions
- **list_qm_users**: List QM system users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Five9 QM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 completed agent evaluations."

**🤖 AI Agent:**
> Fetching evaluations... I found the 5 most recent evaluations, including 'Support Call Review' for Agent Smith (Score: 92) and 'Sales Interaction' for Agent Jones (Score: 85). Would you like to see the details for any of these?

---

**👤 You:**
> "Get the recording link for interaction 'int_12345'."

**🤖 AI Agent:**
> Generating link... I've retrieved a secure temporary link for interaction 'int_12345'. You can listen to the recording here: https://api.five9.com/qm/v1/temp/rec_abc123. Use this for your quality review.

---

**👤 You:**
> "Show me all available evaluation forms."

**🤖 AI Agent:**
> Retrieving forms... You have 3 active evaluation forms: 'General Support Rubric', 'Advanced Technical Troubleshooting', and 'Sales Compliance Checklist'. Which one should I inspect for you?


## Installation & Usage

To install and use the **Five9 QM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/five9-qm](https://vinkius.com/mcp/five9-qm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
