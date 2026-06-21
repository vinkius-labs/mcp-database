# KnowBe4 (KMSAT Reporting) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/knowbe4-kmsat-reporting)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/knowbe4-kmsat-reporting-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/knowbe4-kmsat-reporting-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Audit security awareness — list users, track phishing tests, and monitor risk scores.

## Description
Connect your AI agent to **KnowBe4 KMSAT** to get real-time visibility into your organization's security posture.

### Key Capabilities

- **User Auditing** — List all users and their enrollment status to ensure full coverage of your training programs
- **Phishing Simulation Tracking** — Monitor the results of phishing tests, including click and report rates
- **Risk Score Monitoring** — Access individual and organizational risk scores to identify vulnerabilities
- **Compliance Reporting** — Audit training campaign progress and completion across all departments
- **Group Management** — View group assignments to understand how security policies are being applied

### How to setup

1. Subscribe to this server
2. Log in to KnowBe4, go to **Account Settings** > **Reporting API**, and generate an API Key
3. Enter your key in the configuration panel
4. Start managing your security metrics via natural language


## Available Tools
- **list_users**: Includes user IDs, names, emails, and current status. Essential for auditing user enrollment.

List all users in KnowBe4 KMSAT
- **get_user_details**: Get details for a specific user
- **list_groups**: Useful for auditing training assignments.

List all groups in KnowBe4
- **list_phishing_tests**: Returns test IDs, names, and high-level results.

List phishing security tests
- **get_phishing_test_details**: Get detailed results for a phishing test
- **list_training_campaigns**: Use this to audit compliance and completion rates across the organization.

List security awareness training campaigns
- **get_training_campaign_details**: Get details for a training campaign
- **list_phishing_store_results**: List results for phishing store items
- **get_account_risk_score**: Critical for executive security reporting.

Get the overall account risk score
- **list_user_groups**: List groups for a specific user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KnowBe4 (KMSAT Reporting)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the overall risk score for my KnowBe4 account"

**🤖 AI Agent:**
> The aggregated risk score for your account is currently 42.5 (Medium). This is based on phishing performance, training completion, and overall user behavior.

---

**👤 You:**
> "List the results of our last phishing simulation"

**🤖 AI Agent:**
> Retrieving results for the latest simulation: 'Q1 Compliance Check'. Results: 5% Click Rate, 85% Report Rate, and 0 Data Entry incidents. This is a significant improvement from last month.

---

**👤 You:**
> "Which users have the highest risk scores?"

**🤖 AI Agent:**
> I've identified 5 users with a High Risk Score (>80). These users have failed multiple phishing tests recently. Would you like to see the list and their departments?


## Installation & Usage

To install and use the **KnowBe4 (KMSAT Reporting)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/knowbe4-kmsat-reporting](https://vinkius.com/mcp/knowbe4-kmsat-reporting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
