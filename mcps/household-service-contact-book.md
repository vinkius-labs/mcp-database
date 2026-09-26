# Household Service Contact Book MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-service-contact-book)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize and retrieve service provider profiles, contact methods, and service histories.

## Description
This MCP server acts as a bridge to your household service records. It allows AI agents to manage and retrieve detailed information about service providers, including their contact channels and past service history. Use `get_provider_by_name` to find a specific company, `list_providers_by_service_type` to discover specialists like plumbers or electricians, `get_service_history` to review past work, and `get_contact_details` to find phone numbers or emails.


## Available Tools (4)
- **get_contact_details**: Retrieves all available ways to reach a specific provider
- **get_provider_by_name**: Retrieves the full profile of a service provider using their name
- **get_service_history**: Retrieves a chronological list of past service visits for a specific provider
- **list_providers_by_service_type**: g., Plumbing, Electrical).

Finds all service providers that offer a specific category of service


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Service Contact Book** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who are the plumbers available in my contact book?"

**🤖 AI Agent:**
> The available plumbers are Citywide Plumbing (Account: CP-992) and Reliable Pipes (Account: RP-104).

---

**👤 You:**
> "What was the last service performed by Citywide Plumbing?"

**🤖 AI Agent:**
> The last service by Citywide Plumbing was on March 12, 2024, for a kitchen sink repair.

---

**👤 You:**
> "How can I contact Reliable Pipes?"

**🤖 AI Agent:**
> You can reach Reliable Pipes via phone at 555-0123 or via email at contact@reliablepipes.com.


## ❓ FAQ

**Q: How do I find a plumber?**
You can use the `list_providers_by_service_type` tool and specify 'Plumbing' as the service type to see all available providers.

**Q: How can I see when a provider last visited?**
Use the `get_service_history` tool with the provider's name and their unique account reference to see a chronological list of visits.

**Q: Where can I find a provider's phone number?**
The `get_contact_details` tool provides all available contact channels, such as phone numbers and email addresses, for a specific provider.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-service-contact-book](https://vinkius.com/en/ai-agent-connect/household-service-contact-book)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Service Contact Book** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-service-contact-book` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Service Contact Book** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-service-contact-book": {
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
