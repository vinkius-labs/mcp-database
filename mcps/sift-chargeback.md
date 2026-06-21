# Sift (Chargeback) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sift-chargeback)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sift-chargeback-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sift-chargeback-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Manage fraud prevention and chargebacks via Sift — track user scores, report disputes, and apply decisions directly from any AI agent.

## Description
Connect your **Sift** account to any AI agent and take full control of your fraud protection and chargeback management through natural conversation. Streamline risk analysis and dispute resolution.

### What you can do

- **Chargeback Reporting** — Notify Sift of new chargeback events, including states and reasons natively
- **Fraud Intelligence** — Retrieve real-time fraud scores for users to evaluate transaction risk flawlessly
- **Decision Automation** — Apply manual or automated decisions (e.g., block user, accept order) securely
- **Dispute Oversight** — List and audit the history of decisions and labels applied to any user flawlessly
- **Workflow Visibility** — Access and monitor your configured fraud prevention workflows in real-time
- **Behavioral Tracking** — Log custom events like logins or transactions to refine Sift's machine learning directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Sift REST API Key and Account ID
3. Start managing your fraud protection from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Risk Analysts** — monitor user fraud scores and review chargeback patterns using natural language
- **Trust & Safety Teams** — apply manual decisions and audit user history without opening the dashboard
- **E-commerce Managers** — quickly verify transaction risk and report disputes straight from their chat interface
- **Developers** — verify event integration and scoring data during technical implementation


## Available Tools
- **apply_user_decision**: Apply a manual decision to a user (e.g. block_user)
- **list_user_decision_history**: List the history of decisions applied to a user
- **get_user_fraud_labels**: Retrieve labels (e.g. $bad, $good) applied to a user
- **get_user_fraud_score**: Get the current fraud score for a user
- **list_sift_decisions**: List available decisions (actions) in Sift
- **list_sift_workflows**: List configured fraud prevention workflows
- **report_sift_chargeback**: Report a chargeback event to Sift
- **track_sift_event**: Track a general event (e.g. $login, $transaction) in Sift


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sift (Chargeback)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the fraud score for user 'user_abc_123'?"

**🤖 AI Agent:**
> Checking risk for 'user_abc_123'... The user has a fraud score of 85.2% (High Risk). Sift has labeled this user as '$bad' based on recent transaction patterns.

---

**👤 You:**
> "Report a chargeback for order #999 from user 'user_789' as '$fraud'."

**🤖 AI Agent:**
> Reporting chargeback for order #999... The event has been successfully sent to Sift with the reason '$fraud'. This will update the user's risk profile immediately.

---

**👤 You:**
> "Show me the last 5 decisions applied to user 'user_456'."

**🤖 AI Agent:**
> Retrieving decision history for 'user_456'... I found 2 recent decisions: 'watch_user' (Applied on 2024-03-15) and 'approve_order' (Applied on 2024-02-10).


## Installation & Usage

To install and use the **Sift (Chargeback)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sift-chargeback](https://vinkius.com/mcp/sift-chargeback)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
