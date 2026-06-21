# Portfolio CSV Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/portfolio-csv-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Parse massive CSV exports from brokers like DEGIRO or XTB instantly. Streams financial data locally to prevent AI crashes, returning clean column schemas and sample data.

## Description
When you export your trading history from DEGIRO, XTB, or Interactive Brokers, you get a massive CSV file with thousands of rows. If you upload this directly to Claude, it will exhaust its context window, hallucinate data, and eventually crash.

This MCP acts as your local AI data scientist. It uses a high-speed streaming CSV parser to process the file line-by-line entirely local. Instead of dumping everything into the chat, it intelligently extracts the column headers and a small representative sample. This provides the AI with the exact schema it needs without overwhelming it. The AI can then guide you to write specific aggregation scripts or understand your portfolio safely.

### The Superpowers

- **100% Local Processing:** Your entire financial trading history is read locally.
- **Massive File Support:** Streams CSV files of any size without crashing Node.js or your AI.
- **Smart Schema Extraction:** Automatically detects column headers, separators, and data types.
- **Assistant Ready:** Ask the AI: 'Based on this broker export schema, what columns are available for calculating my P&L?'


## Available Tools (1)
- **parse_portfolio_csv**: Provide the absolute file path.

Parse massive CSV exports from brokers (DEGIRO, XTB, Trading212) locally. Streams the file to prevent RAM crashes and returns column schemas and sample data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Portfolio CSV Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Parse my DEGIRO_export.csv and tell me what data columns I have available to calculate my total dividends."

**🤖 AI Agent:**
> Based on the CSV schema, you have the following columns: Date, Product, ISIN, Description, and Amount. The 'Description' column labels your dividends.

---

**👤 You:**
> "Look at the schema of this broker export and write a Python script for me that sums up all my buy orders."

**🤖 AI Agent:**
> Here is a Python script using pandas that targets the 'Action' and 'Value' columns we just discovered in your CSV file.

---

**👤 You:**
> "How many total rows are in this trading history CSV?"

**🤖 AI Agent:**
> The streaming parser counted exactly 4,521 rows of transaction data.


## ❓ FAQ

**Q: Will it send my entire trading history to the AI?**
No! To protect your privacy and prevent context crashes, it only sends the column headers (the schema), the total row count, and a tiny 20-row sample to the AI.

**Q: What brokers does this work with?**
It works with ANY standard CSV file. Whether it's from DEGIRO, Interactive Brokers, Robinhood, or Trading212, this engine will parse the schema dynamically.

**Q: Can it calculate live market P&L?**
This specific tool focuses purely on parsing the historical CSV data local. For live market prices, a separate API MCP (like Yahoo Finance) would be needed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/portfolio-csv-analyzer](https://vinkius.com/mcp/portfolio-csv-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Portfolio CSV Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `portfolio-csv-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Portfolio CSV Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "portfolio-csv-analyzer": {
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
