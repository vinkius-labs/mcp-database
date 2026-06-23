# FCC Broadcaster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fcc-broadcaster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [media-entertainment](../categories/media-entertainment.md)

Discover radio and television broadcast licensing records and operations across the United States without authentication.

## Description
The **FCC Broadcaster MCP Server** ties your AI agent directly into the operations of United States broadcast media. Ideal for researchers, audiovisual professionals, and licensing analysts, this endpoint allows you to effortlessly search the National Media Bureau databases for active network facilities.

### Core Capabilities

- **TV Station Mapping** — Verify regional television broadcast networks, reviewing signal allocations and operational constraints without hassle.
- **FM & AM Radio Licensing** — Search deep into the local audio ecosystems to extract active broadcast licensing metrics for any registered market.
- **Transparent Gateway** — Fully public, unmetered access to official telecom records, allowing immediate lookup without generating credentials or navigating bureaucratic forms.


## Available Tools (2)
- **get_fm_station_details**: Search for an FM radio broadcast station in the US by Call Sign
- **get_tv_station_details**: Search for a public US Television broadcast station by Call Sign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FCC Broadcaster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the operational details for the radio station WXPN."

**🤖 AI Agent:**
> My search into the FCC broadcast registry confirms that WXPN holds an active license for FM frequency operations, acting as a certified public infrastructure transmission node.

---

**👤 You:**
> "Check if WPVI is currently a licensed TV station."

**🤖 AI Agent:**
> I've checked the television records for WPVI. Yes, it holds an active and licensed status under the official FCC broadcasting matrix.

---

**👤 You:**
> "Identify whether the facility associated with 89.3 FM frequency operations is currently broadcasting."

**🤖 AI Agent:**
> Scanning registered frequencies creatively natively reliably...
The FM facility spanning 89.3 has been formally checked. Current status: Actively licensed to operate optimally safely purely within standard bandwidth constraints natively structurally.


## ❓ FAQ

**Q: Do I need to pay or provide an API Key?**
Absolutely not. The broadcaster database queries operate completely unmetered in the public domain, providing direct agency-to-agent accessibility.

**Q: Can I search for both television and radio networks?**
Yes. This configuration comes with dedicated AI routes for looking up specific Call Signs spanning across the entire FM, AM, and modern TV landscape.

**Q: Are there limits to how many searches I can perform daily?**
As the platform utilizes public regulatory endpoints natively, there are no strict quotas. You can safely poll multiple licensing metrics back-to-back without hitting hard paywalls.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fcc-broadcaster](https://vinkius.com/mcp/fcc-broadcaster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FCC Broadcaster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fcc-broadcaster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FCC Broadcaster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fcc-broadcaster": {
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
