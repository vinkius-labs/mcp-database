# Nimbata MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nimbata)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nimbata-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nimbata-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Track which marketing campaigns generate phone calls with dynamic number insertion and call attribution analytics.

## Description
Connect your **Nimbata** account to any AI agent and take full control of your call tracking orchestration and attribution through natural conversation. Nimbata provides a robust platform for managing inbound calls, and this integration allows you to retrieve call metadata, monitor marketing sources, and manage tracking phone numbers directly from your chat interface.

### What you can do

- **Call & Attribution Orchestration** — List all managed inbound calls and retrieve detailed metadata programmatically, including duration, caller ID, and source attribution.
- **Source & Channel Intelligence** — Access and monitor your marketing tracking sources (Google Ads, Facebook, etc.) and create new ones directly from the AI interface.
- **Number Lifecycle Management** — List all active tracking phone numbers to maintain a clear overview of your communication infrastructure via natural language.
- **Call Deep-Dive** — Retrieve granular details for specific calls to understand context and attribution in real-time using simple AI commands.
- **Operational Monitoring** — Track system health and manage attribution metadata to ensure your marketing funnels are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Nimbata API Key from your dashboard settings
3. Start managing your call tracking from Claude, Cursor, or any MCP-compatible client

No more manual spreadsheet exporting for basic check-ins. Your AI acts as a dedicated call analyst or marketing coordinator.

### Who is this for?

- **Marketing Managers** — quickly retrieve source summaries and monitor attribution health without switching apps.
- **Sales Teams** — automate the retrieval of inbound lead metadata and track call engagement via natural conversation.
- **Developers** — integrate real-time call tracking data and attribution intelligence directly within the chat.


## Available Tools
- **search_calls**: Search calls
- **check_nimbata_status**: Verify connectivity
- **create_source**: Create a tracking source
- **get_call_details**: Get call details
- **get_call_recording**: Get recording
- **get_call_report**: Get call report
- **get_number**: Get number details
- **get_source_report**: Get source report
- **get_source**: Get source details
- **list_calls**: List calls
- **list_numbers**: List tracking numbers
- **list_sources**: List tracking sources


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nimbata** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all tracked calls in Nimbata from today."

**🤖 AI Agent:**
> I've retrieved your calls. You have 5 tracked activities today, including 3 from 'Google PPC' and 2 from 'Organic'. Would you like to see the duration for any of them?

---

**👤 You:**
> "Show me the call tracking sources I have configured and their performance."

**🤖 AI Agent:**
> You have 4 active tracking sources. "Google Ads" generated 89 calls this month (32% conversion rate), "Facebook Campaigns" had 45 calls (28% conversion), "Website Organic" tracked 67 calls (41% conversion), and "Direct Mail" logged 12 calls (50% conversion).

---

**👤 You:**
> "Get the recording and full details for call ID call_7823."

**🤖 AI Agent:**
> Call call_7823 details: Incoming call from +1 (555) 234-5678 on May 10th at 3:42 PM, duration 4m 32s. Source: "Google Ads Brand Campaign". The recording URL has been retrieved and is ready for playback. The caller was matched to tracking number +1 (800) 555-0199.


## Installation & Usage

To install and use the **Nimbata** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nimbata](https://vinkius.com/mcp/nimbata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
