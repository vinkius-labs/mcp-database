# Japanese Train Delay Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/japanese-train-delay-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate Japanese train delay certificate eligibility and excuse categories.

## Description
This MCP server provides deterministic tools to calculate Japanese train delay metrics. It determines if a delay meets the 5-minute threshold for a 'Chien Shoumeisho' (delay certificate) and categorizes the delay into Minor, Moderate, or Significant brackets. Use `calculate_delay_details` to get specific delay minutes and eligibility, `get_excuse_policy_info` to check which delay tiers are accepted for work or school, and `verify_certificate_integrity` to validate a certificate's unique hash.


## Available Tools (3)
- **calculate_delay_details**: Calculates the core metrics of a train delay to determine if a certificate is warranted
- **get_excuse_policy_info**: Provides context on what types of delays are generally accepted by different sectors
- **verify_certificate_integrity**: Validates if a provided hash matches the expected deterministic identifier for a specific delay event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Japanese Train Delay Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My train from JR East was scheduled for 08:00 but actually left at 08:12. Is this delay eligible for a certificate?"

**🤖 AI Agent:**
> The delay is 12 minutes. It is eligible for a certificate and falls into the Moderate delay bracket.

---

**👤 You:**
> "What delay categories are accepted for school?"

**🤖 AI Agent:**
> For school, typically Minor, Moderate, and Significant delay brackets are accepted.

---

**👤 You:**
> "Verify if this hash is valid for JR West on 2024-05-20: abc123hash"

**🤖 AI Agent:**
> The certificate hash is valid for JR West on 2024-05-20.


## ❓ FAQ

**Q: What is the minimum delay required for a certificate?**
Following standard JR rules, a delay must be at least 5 minutes to be eligible for a certificate.

**Q: How can I check if my delay is valid for work?**
You can use the `get_excuse_policy_info` tool to see which delay brackets (Minor, Moderate, or Significant) are typically accepted for the work sector.

**Q: How do I verify a delay certificate hash?**
Use the `verify_certificate_integrity` tool by providing the railway company name, the date of the delay, and the expected hash.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/japanese-train-delay-validator](https://vinkius.com/ai-agent-connect/japanese-train-delay-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Japanese Train Delay Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `japanese-train-delay-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Japanese Train Delay Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "japanese-train-delay-validator": {
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
