# ECB Discovery — Universal Statistical Data Access MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ecb-discovery-universal-statistical-data-access)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ecb-discovery-universal-statistical-data-access-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ecb-discovery-universal-statistical-data-access-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Explore the complete ECB statistical catalog: browse all available dataflows (datasets) and query any ECB SDMX dataset with custom series keys — from exchange rates and monetary aggregates to banking supervision and payment statistics.

## Description
Universal access to all ECB data.

### 2 Tools
- **List Dataflows** — Complete catalog of ECB datasets
- **Query Data** — Any dataflow with custom SDMX keys


## Available Tools
- **list_dataflows**: Each dataflow has a code (e.g., EXR, FM, BSI) and description. Use these codes with the generic query tool to access any ECB data.

List all available ECB statistical dataflows
- **query_ecb_data**: Provide the dataflow code (EXR, FM, BSI, YC, MIR, BKN, etc.) and a SDMX series key. Use list_dataflows to find dataflow codes. Example: dataflow=EXR, key=D.USD.EUR.SP00.A for daily USD/EUR rate.

Query any ECB dataset with a SDMX series key — universal access


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ECB Discovery — Universal Statistical Data Access** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What ECB datasets are available?"

**🤖 AI Agent:**
> 📋 **ECB Dataflows**

| Code | Description |
|------|-------------|
| EXR | Exchange Rates |
| FM | Financial Markets |
| BSI | Balance Sheet Items (M1/M2/M3) |
| MIR | MFI Interest Rates |
| YC | Yield Curves |
| BKN | Banknotes |
| CBD | Consolidated Banking Data |
| SEC | Securities Issues |
| STP | Payment Statistics |

...and many more

---

**👤 You:**
> "Query the Balance Sheet Items (BSI) dataset."

**🤖 AI Agent:**
> I successfully queried the BSI dataset. Here is a summary of the latest balance sheet components and their outstanding amounts for the Euro area, indicating M1, M2, and M3 broad monetary aggregates status.

---

**👤 You:**
> "Extract the latest MFI Interest Rates."

**🤖 AI Agent:**
> The latest MFI Interest Rates (MIR) report has been fetched. The average annualized interest rate for household deposits with an agreed maturity of up to one year has been extracted and tabulated for you.


## Installation & Usage

To install and use the **ECB Discovery — Universal Statistical Data Access** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ecb-discovery-universal-statistical-data-access](https://vinkius.com/mcp/ecb-discovery-universal-statistical-data-access)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
