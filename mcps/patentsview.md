# PatentsView MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/patentsview)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/patentsview-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/patentsview-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Universal US patent intelligence — search patents, inventors, and assignees via AI.

## Description
Equip your AI agent with the definitive source for US patent data through the **PatentsView** MCP server. This integration provides real-time access to the USPTO's massive database of granted patents. Your agent can search for patents by title or keyword, retrieve detailed metadata including abstracts and assignees, and explore information about inventors and their complete portfolios. Whether you are conducting intellectual property research, tracking innovation trends, or auditing corporate assets, your agent acts as a dedicated patent examiner through natural conversation.

### What you can do

- **Patent Search** — Find US patents by keyword, title, or patent number.
- **Inventor Discovery** — Search for inventors and retrieve their complete list of granted patents.
- **Abstract Retrieval** — Access technical summaries and descriptions for thousands of innovations.
- **Innovation Auditing** — Track the patent portfolios of specific individuals or organizations.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start querying US patent data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **IP Professionals & Attorneys** — quickly verify patent details and inventor records.
- **Innovation Researchers** — analyze technology trends and identify key inventors in specific fields.
- **Entrepreneurs & Inventors** — research prior art and explore existing patented technologies.
- **Data Scientists** — access a reliable source of structured patent and innovation data.


## Available Tools
- **get_patent_details**: Get details for a specific patent
- **search_inventors**: Search for inventors by last name
- **search_patents**: Search for US patents by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PatentsView** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for US patents related to 'neural networks'."

**🤖 AI Agent:**
> Searching the PatentsView database... I've found several recent patents related to neural networks, including deep learning frameworks and hardware accelerators. Would you like to see the abstracts or patent numbers?

---

**👤 You:**
> "Find patents by the inventor 'Nikola Tesla'."

**🤖 AI Agent:**
> I've scanned the historical records. I've found several iconic patents assigned to Nikola Tesla, such as the induction motor and alternating current transmission. Which one would you like to inspect?

---

**👤 You:**
> "What are the details for patent number '10000000'?"

**🤖 AI Agent:**
> Retrieving details for patent #10,000,000... This patent is for a 'Coherent frequency-shifted reference beam interferometry' system. It was granted on June 19, 2018. Would you like to read the abstract?


## Installation & Usage

To install and use the **PatentsView** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/patentsview](https://vinkius.com/mcp/patentsview)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
