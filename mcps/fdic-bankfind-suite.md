# FDIC BankFind Suite MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fdic-bankfind-suite)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fdic-bankfind-suite-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fdic-bankfind-suite-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access comprehensive FDIC data on financial institutions, branches, history, and financial performance directly from your AI agent.

## Description
Connect to the **FDIC BankFind Suite** to query public data on US banks and financial institutions. This server provides deep access to the Federal Deposit Insurance Corporation's public records, allowing for detailed analysis of the banking sector through natural conversation.

### What you can do

- **Institution Search** — Find banks by name, certificate number, or location using advanced filtering via `list_institutions`.
- **Branch Mapping** — List specific locations and branches for any financial institution using `list_locations`.
- **Historical Tracking** — Analyze mergers, acquisitions, and structural changes over time with `list_history`.
- **Financial Analysis** — Access Summary of Deposits (SOD) and historic aggregate financial data through `list_sod` and `list_summary`.
- **Failure Records** — Query details on failed institutions and resolution types using `list_failures`.

### How it works

1. Subscribe to this server
2. (Optional) Provide an FDIC API Key for higher rate limits
3. Start querying banking data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts** — instantly retrieve bank performance metrics and historical structural changes.
- **Researchers & Journalists** — track bank failures and industry consolidation trends.
- **Compliance Officers** — verify institution status and branch locations across the US.


## Available Tools
- **list_demographics**: List demographic data related to financial institutions
- **list_failures**: Filter by FAILYR, SAVING, RESTYPE, etc.

List details on failed financial institutions
- **list_financials**: List detailed financial information for institutions
- **list_history**: List details on structure change events (mergers, acquisitions)
- **list_institutions**: Use Elastic Search syntax in filters to search by NAME, CERT, STALP, etc.

List information on financial institutions (banks)
- **list_locations**: Filter by ADDRESS, CITY, COUNTY, ZIP, etc.

List details on financial institution locations and branches
- **list_sod**: List Summary of Deposits (SOD) data
- **list_summary**: List historic aggregate financial and structure data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FDIC BankFind Suite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all banks named 'JPMorgan' using list_institutions."

**🤖 AI Agent:**
> I found several entries for 'JPMorgan'. The primary institution is JPMorgan Chase Bank, National Association (Cert: 628). Would you like to see its branch locations?

---

**👤 You:**
> "List the history of structural changes for bank certificate 628 using list_history."

**🤖 AI Agent:**
> Retrieving history for Cert 628... I've found multiple events, including several mergers with other major banks over the last two decades. Would you like a summary of the most recent acquisition?

---

**👤 You:**
> "Show me a list of failed banks in 2023 using list_failures."

**🤖 AI Agent:**
> In 2023, notable bank failures included Silicon Valley Bank, Signature Bank, and First Republic Bank. I can provide the specific failure dates and resolution details for each.


## Installation & Usage

To install and use the **FDIC BankFind Suite** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fdic-bankfind-suite](https://vinkius.com/mcp/fdic-bankfind-suite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
