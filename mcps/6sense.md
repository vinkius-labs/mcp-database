# 6sense MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/6sense)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/6sense-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/6sense-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Account-based marketing intelligence — identify anonymous visitors, enrich company data, and track intent via AI.

## Description
Connect your **6sense** enterprise account to your AI agent to unlock deep account-based marketing (ABM) insights. From identifying anonymous website traffic to scoring account intent and buying stages, your agent manages B2B intelligence through natural conversation.

### What you can do

- **Company Identification** — Identify anonymous companies visiting your website via IP address analysis
- **Data Enrichment** — Retrieve detailed firmographics and technographics for any account or email address
- **Intent Scoring** — Access AI-driven intent scores (0-100) to prioritize high-value accounts
- **Buying Stages** — Monitor journey stages (Target, Awareness, Consideration, Decision, Purchase) for your target accounts
- **Segment Membership** — Check which marketing segments an account belongs to for better personalization

### How it works

1. Subscribe to this server
2. Enter your 6sense API Token
3. Start prioritizing and enriching your B2B accounts through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Revenue Operations** — automate data flow between 6sense and other sales tools
- **SDRs & BDRs** — research prospect accounts and intent levels before outreach
- **Marketing Managers** — identify which accounts are most engaged with your web content
- **Sales Leaders** — monitor pipeline health and target account journey progress


## Available Tools
- **identify_company**: Identify a company via visitor IP address
- **enrich_company**: g. microsoft.com).

Enrich firmographics and technographics for a domain
- **enrich_person**: Enrich profile information for an email address
- **list_segments**: List marketing segments for a given company


## 💬 Prompt Examples

Here are some examples of how you can interact with the **6sense** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify the company for this IP address: 8.8.8.8"

**🤖 AI Agent:**
> I've analyzed the IP address. It belongs to Google (Alphabet Inc.). Their current intent score is 95 and they are in the 'Purchase' journey stage for your product profile.

---

**👤 You:**
> "Enrich the company data for 'tesla.com'."

**🤖 AI Agent:**
> I've retrieved the data for Tesla, Inc. They are in the Automotive & Energy industry, with over 100,000 employees. They use technologies like Splunk and New Relic. Their intent score is currently 82.

---

**👤 You:**
> "Check which 6sense segments 'microsoft.com' belongs to."

**🤖 AI Agent:**
> Microsoft is currently part of 4 segments: 'Tier 1 Enterprise', 'High Intent - Cloud Solutions', 'Existing Customers', and 'Q4 Expansion Targets'.


## Installation & Usage

To install and use the **6sense** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/6sense](https://vinkius.com/mcp/6sense)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
