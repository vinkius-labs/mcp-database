# Salt Security MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salt-security)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Integrate Salt Security directly with your AI for comprehensive API threat vector discovery, posture management, and active remediation in real-time.

## Description
Connect your AI directly with **Salt Security** to proactively defend your Application Programming Interface (API) environment. Improve API discovery, manage security posture, and remediate threats in real-time through simple conversational prompts.

### What you can do

- **API Inventory & Discovery** — View all auto-discovered APIs in your environment, including unknown or shadow APIs (`get_inventory`). Retrieve schema details, identify exposed sensitive data (PII), and analyze structural drifts (`get_endpoint`).
- **Threat Intelligence & Monitoring** — Monitor active API attacks and business logic abuses as they happen (`get_attacks`). Profile known threat actors to uncover behavioral patterns (`get_attackers`).
- **Active Remediation** — Respond to incidents immediately by triggering blockade commands against attackers, seamlessly passing instructions to your integrated WAFs (`block_attacker`).
- **Posture & Governance Assessment** — Identify design flaws and vulnerabilities before they reach production (`get_posture_vulnerabilities`). Manage OpenAPI (OAS) specifications (`list_oas_specs`, `upload_oas_spec`) and verify active governance rules (`get_governance_policies`).

### How it works

1. Enable the Salt Security integration in your workspace.
2. Navigate to your Salt Security console.
3. Go to the Settings or Administration section and generate a new API Token.
4. Paste this token securely into the configuration fields provided below.
5. Ask the AI: "Are there any known threat actors exploiting our APIs right now?"


## Available Tools (10)
- **block_attacker**: Issues a command to block a specific attacker
- **get_attackers**: Lists known threat actors profiled by Salt
- **get_attacks**: Lists detected malicious API attacks
- **get_endpoint**: Retrieves details for a specific API endpoint
- **get_governance_policies**: Lists active API governance rules
- **get_inventory**: Retrieves the auto-discovered API inventory
- **get_posture_vulnerabilities**: Retrieves identified pre-production design flaws
- **get_system_health**: Checks the health of traffic mirror ingestion
- **list_oas_specs**: Lists all uploaded OpenAPI specifications
- **upload_oas_spec**: Uploads a new OAS/Swagger specification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salt Security** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all auto-discovered APIs including shadow and zombie APIs in our infrastructure."

**🤖 AI Agent:**
> I successfully queried your API inventory. There are currently 32 distinct APIs. Among these, exactly 4 are classified structurally as 'zombie' missing formal documentations.

---

**👤 You:**
> "Are we facing any recent attacks aimed at business logic?"

**🤖 AI Agent:**
> Reviewing your active threat ledger, you have exactly 12 malicious attack events attempting account takeovers targeting primary user authentication web modules currently.

---

**👤 You:**
> "Block attacker 'ATT-992' immediately."

**🤖 AI Agent:**
> The remediation command was actively passed to your Salt Security console. The threat actor profile 'ATT-992' has been assigned an internal blockade rule via integrated gateways.


## ❓ FAQ

**Q: Can the AI forcefully block attackers or does it just view them?**
You can explicitly instruct the AI to use the `block_attacker` tool, which triggers a remediation event across your security infrastructure (e.g., WAF integrations). It provides both visibility and direct active response.

**Q: Does Salt Security allow me to upload spec definitions (OAS) directly from my files via chat?**
Yes, you can upload raw specification content using the `upload_oas_spec` tool for vulnerability testing and validation. Provide the exact OpenAPI content, and Salt will interpret it securely naturally properly successfully cleanly nicely properly natively completely optimally brightly cleanly beautifully actively quickly seamlessly efficiently correctly elegantly faithfully efficiently natively perfectly.

**Q: How frequently is the API inventory auto-discovered?**
Salt maintains a continuous discovery architecture via passive traffic monitoring. This prevents any drift and immediately identifies 'Ghost APIs' when queried using the `get_inventory` capability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salt-security](https://vinkius.com/mcp/salt-security)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salt Security** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salt-security` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salt Security** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salt-security": {
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
