# Richards CRM MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/richards-crm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/richards-crm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/richards-crm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate project management via Richards CRM — manage leads, estimates, and material orders with AI.

## Description
Connect your **Richards Building Supply CRM** account to any AI agent and take full control of your exterior contracting orchestration through natural conversation. Powered by the Construct CRM engine, this integration allows you to retrieve lead metadata, manage project lifecycles, and orchestrate material orders directly from your chat interface.

### What you can do

- **Lead & Prospect Orchestration** — List all managed leads and retrieve detailed profile metadata, including creating new contacts programmatically to ensure your pipeline is always synchronized.
- **Project & Job Lifecycle Management** — Access and monitor active projects and retrieve detailed technical metadata directly from the AI interface to keep your exterior jobs on track.
- **Estimating & Proposals Intelligence** — Access project estimates and monitor proposal statuses to ensure your bidding process is always optimized via natural language.
- **Material Ordering & Invoice Control** — List and retrieve order metadata and invoices to maintain a clear overview of your supply chain and business expenses.
- **Operational Monitoring** — Track employee assignments and manage company profile metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Richards CRM API Key from your account settings
3. Start managing your contracting workflows from Claude, Cursor, or any MCP-compatible client

No more manual order tracking or switching between Material and CRM apps. Your AI acts as a dedicated project coordinator or operations lead.

### Who is this for?

- **Exterior Contractors & Foremen** — quickly retrieve project details and monitor lead status without switching apps.
- **Operations Managers** — automate the management of material orders and track project history via natural conversation.
- **Sales Teams** — streamline the retrieval of estimates and monitor proposal health directly within the chat.


## Available Tools
- **create_lead**: Create a new lead
- **get_company_profile**: Get company profile details
- **get_lead**: Get details for a specific lead
- **get_project**: Get details of a specific project
- **list_employees**: List all employees
- **list_estimates**: List all estimates
- **list_invoices**: List all invoices
- **list_leads**: List all leads
- **list_orders**: List all purchase orders
- **list_projects**: List all projects
- **list_proposals**: List all proposals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Richards CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active leads in my Richards CRM."

**🤖 AI Agent:**
> I've retrieved your leads. You have 5 active prospects including 'John Miller' and 'Chen Residences'. Which one would you like to check the project status for?

---

**👤 You:**
> "Show me all leads in the pipeline with their estimated values and conversion probabilities."

**🤖 AI Agent:**
> 34 leads in the active pipeline. Total estimated value: $2.3M. By stage: New (12, $560K), Contacted (8, $420K), Qualified (6, $480K), Proposal Sent (5, $520K), Negotiation (3, $320K). Hot leads (>80% probability): 5 leads worth $380K. "Meridian Corp" is the highest-value lead at $180K (85% probability, proposal pending). Average pipeline velocity: 28 days from lead to close. Win rate this quarter: 34%. 3 leads are stale (no activity 14+ days).

---

**👤 You:**
> "Create a new lead for TechVentures Inc with a $75,000 estimated project value."

**🤖 AI Agent:**
> Lead created successfully. Company: TechVentures Inc. Primary contact: David Chen (CTO). Email: d.chen@techventures.io. Phone: +1-555-0234. Estimated value: $75,000. Project type: Custom Software Development. Stage: New. Source: Website Form. Assigned to: Sarah (Sales). Lead score: 72/100. Follow-up task created: "Initial discovery call" scheduled for tomorrow at 2 PM. Auto-nurture email sequence activated with 3-email welcome series.


## Installation & Usage

To install and use the **Richards CRM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/richards-crm](https://vinkius.com/mcp/richards-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
