# FMCSA SaferWeb (Carrier Safety) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fmcsa-saferweb-carrier-safety)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fmcsa-saferweb-carrier-safety-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fmcsa-saferweb-carrier-safety-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Access real-time FMCSA carrier safety records, USDOT data, and inspection snapshots directly from the SAFER system.

## Description
Connect your AI agent to the **Federal Motor Carrier Safety Administration (FMCSA)** database to retrieve comprehensive safety snapshots for commercial motor carriers. This server provides direct access to the Safety and Fitness Electronic Records (SAFER) system.

### What you can do

- **Carrier Identification** — Search for carriers by USDOT number, MC/MX number, or legal Company Name to get their official identification data.
- **Safety Snapshots** — Retrieve a concise electronic record of a carrier’s identification, size, and commodity information.
- **Inspection Records** — Access summaries of roadside inspections, including Driver, Vehicle, and Hazmat out-of-service metrics.
- **Crash History** — Query the recorded crash data involving the carrier's fleet over the last 24 months.
- **Safety Ratings** — Check the current safety rating and the date it was issued by the FMCSA.

### How it works

1. Subscribe to this server
2. No complex API keys are required for public data access; simply initialize the connection in the settings
3. Start querying carrier data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Dispatch Teams** — Instantly verify a carrier's safety rating and insurance status before booking a load.
- **Compliance Officers** — Automate the monitoring of fleet safety records and inspection history.
- **Safety Auditors** — Quickly pull snapshot data for reporting and risk assessment without manual web searching.


## Available Tools
- **get_company_snapshot**: Returns parsed text data containing identification, operations, inspections, crashes, and safety rating.

Get a concise electronic record of a carrier’s identification and safety record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FMCSA SaferWeb (Carrier Safety)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the safety snapshot for USDOT number 1234567."

**🤖 AI Agent:**
> I've retrieved the snapshot for USDOT 1234567. The carrier is 'Logistics Express LLC'. They currently have a 'Satisfactory' safety rating with 15 vehicle inspections and 0 crashes reported in the last 24 months.

---

**👤 You:**
> "Search for carrier safety data for 'Swift Transportation' using company name."

**🤖 AI Agent:**
> Searching for 'Swift Transportation'... I found a matching record (USDOT: 54283). The snapshot shows an active status with a fleet of 14,000+ units. Would you like to see the detailed inspection out-of-service percentages?

---

**👤 You:**
> "Check the inspection and crash record for MC number 987654."

**🤖 AI Agent:**
> Querying MC 987654... The electronic record for this carrier indicates 42 driver inspections with a 2.4% out-of-service rate, which is below the national average. There have been 2 tow-away crashes recorded in the past two years.


## Installation & Usage

To install and use the **FMCSA SaferWeb (Carrier Safety)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fmcsa-saferweb-carrier-safety](https://vinkius.com/mcp/fmcsa-saferweb-carrier-safety)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
