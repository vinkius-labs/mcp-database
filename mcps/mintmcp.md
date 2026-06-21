# MintMCP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mintmcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Enterprise MCP Gateway: manage authentication, monitoring, and security guardrails via centralized virtual servers.

## Description
### What you can do

Bring Enterprise Governance seamlessly to your AI Agents with the official MintMCP server connection array:

- **Establish Guardrails** dynamically testing contexts strictly against SOC2 and PI redaction standards natively
- **Discover Virtual Servers** polling explicitly deployed topologies organizing internal plugins
- **Audit Executions securely** dumping complete logic access events into security metrics natively
- **Deploy Centralized Proxies** routing agent workflows securely to down-stream architectures
- **Query RBAC tool policies** mapping rigid logic controls determining explicitly who executes a specific function
- **Revoke Tokens Instantly** isolating logic compromised connections safely from the main host

### How it works

1. **Procure your MintMCP variables**, declaring both your global Tenant ID matrix and the primary API Token
2. **Set the context engine limits** restricting the AI solely to native execution bounds
3. **Request telemetries and runs** resolving exactly matching endpoints to audit logic executions across isolated nodes
4. **Govern workflows safely** without compromising literal organizational compliance standards

### Who is this for?

Explicitly designed mapping towards **Security Engineering Leads**, **Enterprise Platform Admins**, and **Compliance Matrices** operating LLMs securely. If restricting AI actions is a requirement, integrating MintMCP handles it frictionlessly.


## Available Tools
- **mintmcp_eval_guardrail**: Pass structural parameter string checking via unified security AI PI-redaction guardrail engines
- **mintmcp_fetch_audit_logs**: Dump systematic telemetries logging SOC2 matrix accesses tracking execution
- **mintmcp_get_tool_policy**: Fetch the definitive SOC2 governance and RBAC parameters restricting one logic integration
- **mintmcp_get_virtual_server**: Extract exact configuration patterns of one unique Virtual Server schema
- **mintmcp_list_available_tools**: Audit underlying tools currently approved locally inside a Virtual Server
- **mintmcp_list_virtual_servers**: List all Virtual Server proxy abstractions grouping tools functionally
- **mintmcp_revoke_access_token**: Sunder seamlessly a runtime session abstraction resolving an active OAuth flow
- **mintmcp_run_tool_action**: Proxy explicitly an execution logic stream safely hitting the native integrations running behind the gateway


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MintMCP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the exact list of available virtual servers configured on my organization proxy natively."

**🤖 AI Agent:**
> Parsing proxy layers (`list_virtual_servers`). Resulting execution captured 3 dynamic topologies natively mapped to your access limitations completely securely.

---

**👤 You:**
> "Verify the PI redaction guardrails against the textual payload 'Transfer funds using account ABC'."

**🤖 AI Agent:**
> Sending diagnostic limits (`eval_guardrail`). Gateway engines returned cleanly verifying policies successfully triggered catching no critical parameters mapping explicitly internally.

---

**👤 You:**
> "Poll the last 10 security audit execution logs from our native environment bounds."

**🤖 AI Agent:**
> Fetching limit bounds array naturally spanning telemetry limits (`fetch_audit_logs`). Extracted explicit logging histories mapping exclusively native connections flawlessly secure.


## ❓ FAQ

**Q: Can I test payload parameters through the security Guardrails offline?**
Yes, mapping direct values through `eval_guardrail` runs simulated queries bypassing the actual downstream proxy directly into the evaluation loop.

**Q: Are explicit SOC2 Audit Logs available natively to query via this agent integration?**
Yes! Utilize `fetch_audit_logs` limiting explicitly standard parameters to unpack all tool executions securely bounded inside your tenant matrix natively.

**Q: How do virtual servers separate functional tools proxy instances natively?**
By polling `list_available_tools` against a specific server ID, you extract rigidly grouped schemas bounded solely to that environment parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mintmcp](https://vinkius.com/mcp/mintmcp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MintMCP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mintmcp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MintMCP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mintmcp": {
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
