# Sift (Chargeback) MCP Server

Manage fraud prevention and chargebacks via Sift — track user scores, report disputes, and apply decisions directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sift-chargeback)

## Overview
**Category:** security-compliance
**Tools Count:** 8

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


## Installation & Usage

To install and use the **Sift (Chargeback)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sift-chargeback](https://vinkius.com/mcp/sift-chargeback)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
