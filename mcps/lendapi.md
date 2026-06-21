# LendAPI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lendapi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lendapi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lendapi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage loan applications, borrower profiles, and credit decisioning via the LendAPI REST API.

## Description
Connect your **LendAPI** account to any AI agent to automate your loan origination and management workflows. This MCP server enables your agent to interact with borrower profiles, manage loan applications, and trigger automated credit decisioning directly from natural language interfaces.

### What you can do

- **Borrower Oversight** — List and retrieve detailed profiles for all registered borrowers in your system
- **Application Lifecycle** — List, retrieve, and create loan application drafts while monitoring their current status
- **Credit Decisioning** — Submit applications for automated credit review and trigger AI/ML risk assessments
- **Data Standardization** — Retrieve valid picklist values for purposes, industries, and asset types to ensure data quality
- **Onboarding Automation** — Create new borrower records and manage their associated loan requests seamlessly

### How it works

1. Subscribe to this server
2. Enter your LendAPI API Key (Bearer Token)
3. Start managing your digital lending operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Lending Managers** — Monitor application pipelines and borrower statuses via simple natural language commands
- **Underwriters** — Quickly retrieve applicant metadata and financial history without leaving your dev tools
- **Fintech Developers** — Integrate loan origination logic and borrower management into your custom fintech applications


## Available Tools
- **list_loan_applications**: List all loan applications
- **list_borrowers**: List all borrower profiles
- **create_loan_application**: Requires a JSON body with application details.

Create a new loan application
- **create_new_borrower**: Requires a JSON body with profile details.

Create a new borrower profile
- **get_application_details**: Get details for a specific loan application
- **get_borrower_details**: Get details for a specific borrower
- **get_lendapi_picklists**: Retrieve valid picklist values for metadata fields
- **submit_loan_application**: Submit a loan application for decisioning


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LendAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all borrowers in my LendAPI account."

**🤖 AI Agent:**
> I've retrieved your borrowers. You have 12 registered profiles, including 'John Smith', 'Alice Doe', and 'Robert Brown'. Which one would you like to inspect?

---

**👤 You:**
> "Show details for loan application ID 'APP-12345'."

**🤖 AI Agent:**
> I've fetched application APP-12345. It's currently in 'Underwriting' status for a personal loan of $5,000.00. The primary borrower is 'John Smith'.

---

**👤 You:**
> "Submit application 'APP-12345' for a final credit decision."

**🤖 AI Agent:**
> Successfully submitted application APP-12345 for decisioning. The automated engine is now reviewing the risk profile and generating a credit outcome.


## Installation & Usage

To install and use the **LendAPI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lendapi](https://vinkius.com/mcp/lendapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
