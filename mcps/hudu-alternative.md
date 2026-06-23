# Hudu MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hudu-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Document your IT infrastructure with password vaults, knowledge bases, and asset tracking built for managed service providers.

## Description
Connect your **Hudu** instance to any AI agent and manage your IT documentation through natural conversation.

### What you can do

- **Company Management** — List all client companies, inspect profiles, and create new company records
- **Asset Tracking** — Browse all assets (servers, workstations, network devices), filter by company, inspect details, and create new asset records with tags
- **Password Vault** — List stored passwords filtered by company, and securely retrieve individual password entries with secrets
- **Knowledge Base** — Browse all articles and read full content with metadata for any specific article
- **Procedures & Checklists** — List all procedures filtered by company and inspect detailed steps for operational checklists

### How it works

1. Subscribe to this server
2. Enter your Hudu Instance URL and API Key
3. Start managing IT documentation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **MSPs (Managed Service Providers)** — access client documentation, passwords, and asset inventories without opening the Hudu portal
- **IT Administrators** — track assets, review procedures, and manage knowledge base articles through AI
- **Support Engineers** — quickly retrieve client passwords, asset details, and troubleshooting procedures during incidents


## Available Tools (12)
- **get_article**: Get details for a specific article
- **get_asset**: Get details for a specific asset
- **get_company**: Get details for a specific company
- **get_password**: Get details for a specific password
- **get_procedure**: Get details for a specific procedure
- **list_articles**: List knowledge base articles
- **list_assets**: Can be filtered by company ID.

List assets
- **list_companies**: List all companies in Hudu
- **list_passwords**: Can be filtered by company ID.

List passwords
- **list_procedures**: Can be filtered by company ID.

List procedures
- **create_asset**: Requires asset name and company ID.

Create a new asset
- **create_company**: Requires a name.

Create a new company


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hudu** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all companies and the assets for 'Acme Corp', then retrieve the admin password."

**🤖 AI Agent:**
> Companies: 18 clients managed. Acme Corp (company_12): 14 assets. Assets: 1) 'DC-SRV-01' (Server, Windows Server 2022, tag: DC). 2) 'DC-SRV-02' (Server, Ubuntu 22.04, tag: Backup). 3) 'FW-01' (Firewall, Fortinet, tag: Core). 4) 'SW-CORE-01' (Switch, Cisco 9300). 5-14) 10 workstations. Passwords for Acme Corp: 6 entries. 'Domain Admin' password (pwd_089): Username: admin@acmecorp.local, Password: ●●●●●●●●●●●●, Last rotated: Apr 1, 2025. ⚠️ Password is 25 days old — consider rotating. Would you like to see procedures or knowledge base articles for Acme?

---

**👤 You:**
> "Search the knowledge base for articles about VPN setup and show the firewall procedures."

**🤖 AI Agent:**
> Knowledge base articles: 34 total. VPN-related: 1) 'Site-to-Site VPN Configuration — Fortinet' (article_045, updated Mar 15). Content: Step-by-step guide for configuring IPsec VPN tunnels between Fortinet firewalls, including Phase 1/2 parameters, routing, and NAT traversal. 2) 'Remote Access VPN — FortiClient Setup' (article_046). 3) 'VPN Troubleshooting Guide' (article_052). Firewall procedures: 1) 'Monthly Firewall Rule Audit' (proc_012, 8 steps, company: All clients). Steps: 1. Export current ruleset → 2. Review unused rules → 3. Check expired policies → 4. Validate NAT rules → 5. Test connectivity → 6. Document changes → 7. Backup config → 8. Sign off. Would you like to read a full article or create a new asset?

---

**👤 You:**
> "Create a new company 'TechStart Inc' and add a server asset to it."

**🤖 AI Agent:**
> Company created! Name: TechStart Inc, ID: company_19. You now have 19 managed clients. Asset created! Name: 'TS-SRV-01', Company: TechStart Inc (company_19), Tag: 'Production', ID: asset_287. The asset is now linked to TechStart Inc. Next steps: you may want to add passwords for this client and create onboarding procedures. Would you like to add passwords or create more assets?


## ❓ FAQ

**Q: Can I retrieve stored passwords for a specific client?**
Yes. Use `list_passwords` with an optional `company_id` to filter passwords by client. Then use `get_password` with a specific password ID to retrieve the full entry including the secret. Use `list_companies` to find the company ID first.

**Q: Does Hudu require a custom instance URL?**
Yes. Hudu is self-hosted or uses dedicated instances, so you need to provide your **Instance URL** (e.g., `https://your-company.huducloud.com`) along with the **API Key**. The API Key is sent via the `x-api-key` header (not Bearer), and all API calls are routed to `{instanceUrl}/api/v1`.

**Q: Can I track all assets for a specific company?**
Yes. Use `list_assets` with the `company_id` parameter to retrieve all assets (servers, workstations, network devices) for a specific client. Use `get_asset` for detailed specifications and tags. Use `create_asset` to add new assets with a name, company ID, and optional asset tag.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hudu-alternative](https://vinkius.com/mcp/hudu-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hudu** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hudu-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hudu** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hudu-alternative": {
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
