# Paperspace MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paperspace)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Provision and track powerful GPU workloads via Paperspace — list compute instances, fetch active deployments, trace team projects, and query Gradient environments via AI.

## Description
Bring **DigitalOcean Paperspace Cloud Insights** directly into your AI workflows. By bridging directly with your AI compute environments, this integration tracks active deep learning machines, traces deployment logic natively, maps active Jupyter notebooks acting as Gradient limits, and exports the strict profile bounds applied across your data-science operations.

### What you can do

- **Compute Core Engine** — Identify heavily modified REST boundaries targeting physical core/GPU machines extracting memory schemas and storage constraints gracefully
- **Project Modeling** — Trace collaborative groupings checking native team logic and limits defining exactly how GPU units map globally into discrete Project clusters
- **Notebook Insights** — Query raw Jupyter notebooks attached strictly to the deep logic Gradient models determining idle constraints
- **Deployment Workloads** — Check serverless API container logs determining container availability

### How it works

1. Subscribe to this server
2. Enter your Paperspace API Key
3. Start monitoring GPU footprints globally using Claude, Cursor, or any MCP container

### Who is this for?

- **AI Developers** — instantly examine GPU allocations on heavy models cleanly mapping limits from chat spaces
- **Infrastructure Ops** — fetch disconnected deployments verifying which container APIs are active natively
- **ML Researchers** — track specific AI lab setups investigating Jupyter limits and RAM boundaries instantly


## Available Tools
- **list_machines**: Identify bounded Compute resources inside the Headless Paperspace limits
- **get_machine_details**: Perform structural extraction of properties driving active Instance logic
- **list_deployments**: Retrieve explicit Cloud logging tracing explicit Deploy targets
- **list_notebooks**: Inspect deep internal arrays mitigating specific AI workload limits
- **list_projects**: Enumerate explicitly attached structured rules exporting active Team limits
- **get_user_details**: Identify precise active arrays spanning native Identity Auth


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paperspace** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan Paperspace for any currently active deployed Core machines."

**🤖 AI Agent:**
> Successfully queried physical limit layers. Found 2 virtual Core instances. Instance `ps1aaq4`: P4000 GPU (Off). Instance `ps38jxx`: RTX5000 GPU (Running) allocated 30GB of internal RAM. Should I describe `ps38jxx` deeply?

---

**👤 You:**
> "Execute an inventory sweep over active Gradient Jupyter Notebooks running in production."

**🤖 AI Agent:**
> Tapped native AI layer arrays determining 1 Gradient environment running explicitly in the background. Token id `nxxx`. Attached to deep learning target container environment. Status: Provisioned. The workspace maps exclusively back to 'Computer Vision Team 1'.

---

**👤 You:**
> "Show exactly which users are tied down to my native Paperspace environment."

**🤖 AI Agent:**
> Parsed global arrays confirming absolute account identities. Account belongs to "Team Vinkius". Billing Profile: Active Card. Support Plan: Developer. Storage constraint ceiling set to strictly 2000 GB.


## ❓ FAQ

**Q: Are Paperspace Core machines dynamically mapped?**
Yes. The `list_machines` query returns deeply structured attributes associated exactly with the base compute objects provisioning storage arrays, IPs, and states running natively over Paperspace Core.

**Q: Can I spin up new Jupyter Gradient instances?**
Currently, this module focuses strictly on dynamic observability — pulling down Notebooks arrays, Teams constraints, and extracting native deploy mapping contexts. Write operations to spin up environments are out-of-scope for read workflows.

**Q: How do I fetch the resource specs belonging to a specific ID?**
After listing the overall arrays, provide the `psxxxxxx` ID identifier securely to the `get_machine_details` extractor to generate raw hardware limitations mapped logically inside that node.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paperspace](https://vinkius.com/mcp/paperspace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paperspace** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `paperspace` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paperspace** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paperspace": {
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
