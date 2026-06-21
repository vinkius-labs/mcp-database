# InvestorLift MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/investorlift)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/investorlift-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/investorlift-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Automate real estate deal sourcing via InvestorLift — list marketplace deals, manage your buy box criteria, and message sellers directly from any AI agent.

## Description
Connect your **InvestorLift** account to any AI agent to streamline your real estate investment workflow. Find off-market deals, analyze property data, and communicate with wholesalers through natural language.

### What you can do

- **Marketplace Access** — Browse and filter thousands of real estate deals using `list_deals` by location and price.
- **Deal Analysis** — Get deep insights into specific properties, including pricing and metadata, with `get_deal`.
- **Investment Strategy** — Retrieve and update your `buy_box` criteria to ensure the AI understands your target ROI and preferred locations.
- **Direct Communication** — Use `send_message` to start negotiations or ask questions to sellers immediately.

### How it works

1. Subscribe to this server
2. Enter your InvestorLift API Key
3. Start sourcing and managing real estate deals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Real Estate Investors** — quickly find deals that match your specific criteria without manual searching
- **Wholesalers & Agents** — analyze market inventory and communicate with sellers directly from your workflow
- **Investment Analysts** — pull property data into your analysis tools via AI conversation


## Available Tools
- **list_deals**: List available deals in the marketplace
- **get_buy_box**: Get your current buy box criteria
- **get_deal**: Get detailed information about a specific deal
- **send_message**: Send a message to a seller regarding a specific deal
- **update_buy_box**: Update your buy box criteria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **InvestorLift** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available deals in Houston, Texas with a maximum price of $300,000."

**🤖 AI Agent:**
> I've found 3 deals in Houston under $300k. One is a 3-bed fixer-upper (ID: 55432) for $245,000. Would you like more details on any of these?

---

**👤 You:**
> "What are my current investment criteria in my buy box?"

**🤖 AI Agent:**
> Your current buy box is set to target Single Family homes in Florida and Georgia with a minimum ROI of 12% and a price range between $150k and $450k.

---

**👤 You:**
> "Send a message to the seller of deal 98765 saying I am interested in a cash offer."

**🤖 AI Agent:**
> Message sent successfully to the seller of deal 98765. I've let them know you're interested in making a cash offer.


## Installation & Usage

To install and use the **InvestorLift** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/investorlift](https://vinkius.com/mcp/investorlift)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
