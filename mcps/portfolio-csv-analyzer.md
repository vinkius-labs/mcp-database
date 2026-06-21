# Portfolio CSV Analyzer MCP Server

Parse massive CSV exports from brokers like DEGIRO or XTB instantly. Streams financial data locally to prevent AI crashes, returning clean column schemas and sample data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/portfolio-csv-analyzer)

## Overview
**Category:** data-analytics
**Tools Count:** 1

## Description
When you export your trading history from DEGIRO, XTB, or Interactive Brokers, you get a massive CSV file with thousands of rows. If you upload this directly to Claude, it will exhaust its context window, hallucinate data, and eventually crash.

This MCP acts as your local AI data scientist. It uses a high-speed streaming CSV parser to process the file line-by-line entirely local. Instead of dumping everything into the chat, it intelligently extracts the column headers and a small representative sample. This provides the AI with the exact schema it needs without overwhelming it. The AI can then guide you to write specific aggregation scripts or understand your portfolio safely.

### The Superpowers

- **100% Local Processing:** Your entire financial trading history is read locally.
- **Massive File Support:** Streams CSV files of any size without crashing Node.js or your AI.
- **Smart Schema Extraction:** Automatically detects column headers, separators, and data types.
- **Assistant Ready:** Ask the AI: 'Based on this broker export schema, what columns are available for calculating my P&L?'


## Available Tools
- **parse_portfolio_csv**: Provide the absolute file path.

Parse massive CSV exports from brokers (DEGIRO, XTB, Trading212) locally. Streams the file to prevent RAM crashes and returns column schemas and sample data


## Installation & Usage

To install and use the **Portfolio CSV Analyzer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/portfolio-csv-analyzer](https://vinkius.com/mcp/portfolio-csv-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
