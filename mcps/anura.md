# Anura MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/anura)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/anura-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/anura-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Ad fraud detection MCP server. Validate visitors in real-time and manage fraud reports via Anura.io.

## Description
Protect your advertising spend with the **Anura MCP Server**. This integration allows your AI agent to interact directly with Anura.io's advanced fraud detection engine. Validate visitor traffic in real-time, monitor campaign health, and retrieve detailed fraud reports without leaving your workspace.

### What you can do

- **Real-Time Validation** — Check if a visitor (IP + User-Agent) is 'Good', 'Warning', or 'Bad' instantly.
- **Campaign Monitoring** — List monitored campaigns and traffic sources to identify where fraud is coming from.
- **Detailed Reporting** — List, retrieve, and download comprehensive fraud reports for deep analysis.
- **Fraud Statistics** — Get summarized statistics for specific time ranges to track fraud trends over time.
- **System Health** — Check Anura's current system status to ensure reliable monitoring.

### How it works

1. Subscribe to this server
2. Provide your Anura Instance ID and Secret Key
3. Start validating traffic or analyzing fraud patterns through your AI chat interface.

### Who is this for?

- **Ad Ops Managers** — Quickly verify if a suspicious traffic source is valid.
- **Performance Marketers** — Monitor fraud rates across different campaigns in real-time.
- **Data Analysts** — Automate the retrieval of fraud reports for custom internal dashboards.


## Available Tools
- **get_system_status**: Check Anura system status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Anura** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate visitor with IP 1.2.3.4 and User-Agent 'Mozilla/5.0...'"

**🤖 AI Agent:**
> I've checked the visitor data with Anura. The result is 'Good', meaning the traffic is likely legitimate and non-fraudulent.

---

**👤 You:**
> "Show me the fraud statistics for the last 7 days."

**🤖 AI Agent:**
> I've pulled the fraud stats for the last week. Your overall fraud rate is 2.4%, with most 'Bad' traffic coming from source 'Network_A'.

---

**👤 You:**
> "List my active campaigns in Anura."

**🤖 AI Agent:**
> You have 5 active campaigns being monitored: 'Spring_Launch', 'Summer_Sale', 'Retargeting_Global', 'New_User_Offer', and 'Brand_Awareness'.


## Installation & Usage

To install and use the **Anura** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anura](https://vinkius.com/mcp/anura)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
