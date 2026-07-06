# Troops MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/troops)
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


## Available Tools (7)
- **create_candidate**: Register a new candidate
- **get_candidate**: Get candidate details
- **submit_timesheet**: Submit a time sheet
- **create_job**: Create a new job offer
- **generate_contract**: Generate a contract
- **list_jobs**: Can be filtered by status.

List job offers
- **sign_contract**: Sign a contract


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


## ❓ FAQ

**Q: How can I see all currently published job offers?**
You can use the `list_jobs` tool. You can also filter the results by status, such as 'published', to see only active listings.

**Q: Is it possible to register a new candidate directly through the AI?**
Yes! Use the `create_candidate` tool by providing the candidate's first name, last name, and email address to add them to your Troops database.

**Q: How do I submit hours worked for a specific contract?**
Use the `submit_timesheet` tool. You will need to provide the `contract_id` and a JSON array representing the daily hours worked.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/troops](https://vinkius.com/mcp/troops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Troops** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `troops` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Troops** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "troops": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
