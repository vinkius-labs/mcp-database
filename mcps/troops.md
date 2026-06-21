# Troops MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/troops)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/troops-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/troops-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate HR and recruitment workflows via Troops — manage job offers, candidates, contracts, and timesheets directly from your AI agent.

## Description
Connect your **Troops** account to any AI agent to streamline your recruitment and HR operations through natural conversation.

### What you can do

- **Job Management** — List existing job offers or create new ones with specific locations and dates using `list_jobs` and `create_job`.
- **Candidate Pipeline** — Register new candidates and retrieve detailed profiles instantly with `create_candidate` and `get_candidate`.
- **Contract Automation** — Generate legal contracts for specific jobs and trigger electronic signature processes via `generate_contract` and `sign_contract`.
- **Time Tracking** — Submit and manage timesheets for active contracts to ensure accurate payroll using `submit_timesheet`.

### How it works

1. Subscribe to this server
2. Enter your Troops API Key
3. Start managing your workforce from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — quickly list open positions and candidate details without switching tabs.
- **Recruiters** — automate the registration of new talent and contract generation.
- **Operations Teams** — streamline the submission of hours and contract signing workflows.


## Available Tools
- **create_candidate**: Register a new candidate
- **create_job**: Create a new job offer
- **generate_contract**: Generate a contract
- **get_candidate**: Get candidate details
- **list_jobs**: Can be filtered by status.

List job offers
- **sign_contract**: Sign a contract
- **submit_timesheet**: Submit a time sheet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Troops** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all published job offers in the system."

**🤖 AI Agent:**
> I've retrieved the published jobs. There are currently 3 active offers: 'Senior Frontend Developer' (ID: job_001), 'Product Manager' (ID: job_002), and 'HR Specialist' (ID: job_003).

---

**👤 You:**
> "Register a new candidate: Alice Smith, alice.smith@email.com."

**🤖 AI Agent:**
> Alice Smith has been successfully registered as a candidate with ID: cand_987. You can now use this ID to generate contracts or view her profile.

---

**👤 You:**
> "Generate a contract for candidate cand_987 for job job_001 with a salary rate of 55."

**🤖 AI Agent:**
> The contract has been generated for Alice Smith for the Senior Frontend Developer position. Contract ID: ct_456. Would you like me to trigger the electronic signature process now?


## Installation & Usage

To install and use the **Troops** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/troops](https://vinkius.com/mcp/troops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
