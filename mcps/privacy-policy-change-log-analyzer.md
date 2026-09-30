# Privacy Policy Change Log Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/privacy-policy-change-log-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Compares privacy policy versions to identify added, removed, or changed clauses and service impacts.

## Description
This MCP server provides specialized tools for analyzing textual modifications between different versions of a privacy policy. It allows users to use `compare_policy_versions` to detect specific additions, removals, and modifications in policy clauses. Additionally, it can use `identify_service_impact` to flag which business services require manual review based on a configurable change threshold. It also provides access to the full policy content via `fetch_policy_version` and the list of valid thematic categories through `get_policy_categories`.


## Available Tools (4)
- **compare_policy_versions**: Identifies all additions, removals, and modifications between two specific policy versions
- **fetch_policy_version**: Retrieves the full content of a specific policy version by its identifier or date
- **get_policy_categories**: Retrieves the valid list of thematic categories used for organizing clauses
- **identify_service_impact**: Determines which business services must be reviewed based on the magnitude of the policy changes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Privacy Policy Change Log Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare the policy version 'v1' with 'v2' and tell me what changed."

**🤖 AI Agent:**
> The comparison shows that one clause in 'Data Collection' was added and one clause in 'Third-Party Sharing' was modified.

---

**👤 You:**
> "Which services are impacted if the change ratio is 0.1?"

**🤖 AI Agent:**
> Based on the current change log, the 'Advertising Service' is flagged for review.

---

**👤 You:**
> "What are the valid categories for organizing policy clauses?"

**🤖 AI Agent:**
> The valid categories are Data Collection, User Rights, Third-Party Disclosure, and Data Retention.


## ❓ FAQ

**Q: How do I compare two different policy versions?**
You can use the `compare_policy_versions` tool by providing the JSON representations of both the old and new policy versions.

**Q: What determines if a service is flagged for review?**
A service is flagged if the ratio of changes (added, removed, or modified clauses) in its associated categories exceeds the threshold provided to `identify_service_impact`.

**Q: Can I retrieve the full text of a specific policy?**
Yes, use the `fetch_policy_version` tool with the specific version identifier to retrieve the complete content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/privacy-policy-change-log-analyzer](https://vinkius.com/en/ai-agent-connect/privacy-policy-change-log-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Privacy Policy Change Log Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `privacy-policy-change-log-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Privacy Policy Change Log Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "privacy-policy-change-log-analyzer": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
