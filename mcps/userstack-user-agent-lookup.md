# UserStack User-Agent Lookup MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/userstack-user-agent-lookup)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/userstack-user-agent-lookup-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/userstack-user-agent-lookup-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Universal User-Agent intelligence — detect devices, browsers, and OS via AI.

## Description
Equip your AI agent with real-time browser and device intelligence through the **UserStack** MCP server. This integration provides instant parsing of User-Agent strings to identify the device type (mobile, desktop, tablet), brand, operating system, and browser version. Your agent can also detect crawlers and bots with high precision. Whether you are auditing web traffic, personalizing user experiences, or researching device distributions, your agent acts as a dedicated technical analyst through natural conversation.

### What you can do

- **UA Parsing** — Decode complex User-Agent strings into structured device and browser data.
- **Bot Detection** — Identify if a request is coming from a human user or a search engine crawler.
- **Technical Auditing** — Verify the OS and browser capabilities of specific web clients.
- **Device Profiling** — Retrieve brand and model information for mobile and desktop systems.

### How it works

1. Subscribe to this server
2. Enter your UserStack Access Key (get it at userstack.com)
3. Start detecting User-Agents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web Developers** — quickly debug and analyze User-Agent data for testing.
- **Security Analysts** — identify suspicious agents or bot activity in web logs.
- **Digital Marketers** — profile the technology used by website visitors.
- **Operations Teams** — automate the classification of incoming web requests.


## Available Tools
- **detect_user_agent**: Identify device and browser from User-Agent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UserStack User-Agent Lookup** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Detect this User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36"

**🤖 AI Agent:**
> Parsing User-Agent... I've identified this as a Desktop user on Windows 10 using Google Chrome version 91. It is not a search engine crawler.

---

**👤 You:**
> "Is this a bot? 'Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)'"

**🤖 AI Agent:**
> Checking agent... Yes, this is identified as Googlebot version 2.1, a verified search engine crawler from Google.

---

**👤 You:**
> "Identify the device brand for this UA: 'Mozilla/5.0 (iPhone; CPU iPhone OS 14_6 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.1.1 Mobile/15E148 Safari/604.1'"

**🤖 AI Agent:**
> Analyzing... This User-Agent belongs to an Apple iPhone running iOS 14.6. The browser is Safari mobile version 14.1.1.


## Installation & Usage

To install and use the **UserStack User-Agent Lookup** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/userstack-user-agent-lookup](https://vinkius.com/mcp/userstack-user-agent-lookup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
