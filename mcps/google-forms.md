# Google Forms MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-forms)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/google-forms-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/google-forms-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Analyze datasets actively — list active Google Forms, query exact responses, and fetch metadata programmatically.

## Description
Connect your **Google Forms** infrastructure to a conversational AI assistant. You will bypass the need to constantly refresh CSV downloads or read through dense graphical charts by chatting directly with the pipeline stream.

### What you can do

- **Forms Aggregation** — List available forms by file ID to pinpoint exact surveys you are running over your customer base
- **Rapid Metadata Validation** — Inspect the schema of each active form directly to verify exactly what questions your marketing team is querying
- **Live Response Streaming** — Pull raw answering data and aggregated insights of all recent form submits right inside your chat environment seamlessly

### How it works

1. Install and subscribe to the server hook
2. Authorize via standard OAuth 2.0 mechanisms pointing to Workspace
3. Execute advanced read commands querying from your form matrix

### Who is this for?

- **Marketers & Analysts** — run quick summarization on customer NPS score trends without diving into raw CSV grids daily
- **Event Coordinators** — retrieve exact answers and confirmations from attendees using targeted IDs over text


## Available Tools
- **get_form_metadata**: Get metadata and structure of a Google Form
- **get_form_responses**: Get all responses for a Google Form


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Forms** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Read the form metadata and structure for the Form ID 'abc123xyz'."

**🤖 AI Agent:**
> I've fetched the structure. The active Form is titled 'Post-Event Feedback 2024'. It contains 4 explicit questions, including 'Rate your experience (1-10)' and 'Freeform Comments'.

---

**👤 You:**
> "Fetch the responses recorded today in the Sales Survey (Form ID abc). Summarize the general satisfaction."

**🤖 AI Agent:**
> I've captured 22 recent responses. Across those payloads, the prevalent satisfaction score hovers between 8 and 9. Top positive highlight: 'Fast customer service'. Negative outliers point out a lack of documentation.

---

**👤 You:**
> "List all active form instances under my account to find the latest specific quiz run."

**🤖 AI Agent:**
> Search initialized. Under your root index I discovered two forms matching normal schemas: 'Marketing Q1 Trends' (ID 4122) and 'Staff Quiz Baseline' (ID 198a). Which one should I focus on?


## Installation & Usage

To install and use the **Google Forms** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-forms](https://vinkius.com/mcp/google-forms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
