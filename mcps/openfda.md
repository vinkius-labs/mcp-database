# openFDA MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openfda)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openfda-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openfda-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access the powerful openFDA databases for drug adverse events, food recalls, and medical device safety reports globally.

## Description
The **openFDA MCP Server** provides direct, zero-auth access to the United States Food and Drug Administration (FDA) regulatory databases. This server allows your AI agent to construct complex pharmacological queries and retrieve public health data in real-time.

### Core Capabilities

- **Drug Adverse Events** — Investigate documented side effects, medication errors, and quality complaints across millions of historical patient records.
- **Food Safety Recalls** — Keep track of active and historical FDA enforcement reports, including outbreaks of pathogens like Salmonella or Listeria.
- **Medical Device Safety (MAUDE)** — Monitor injuries, malfunctions, and deaths associated with medical devices.
- **Advanced Search Capabilities** — All tools accept raw query syntax, giving your AI agent absolute freedom to perform highly granular, multi-variable analytical research.

Ideal for healthcare researchers, compliance officers, and public safety analysts requiring deep programmatic data scraping without the overhead of API key management.


## Available Tools
- **query_drug_events**: g., patient.drug.medicinalproduct:"ASPIRIN", patient.reaction.reactionmeddrapt:"HEADACHE"). The dataset contains reports of adverse events, medication errors, and product quality complaints. Max limit is 100.

Query the openFDA Drug Adverse Events database using Lucene syntax
- **query_food_recalls**: Examples: reason_for_recall:"salmonella", status:"Ongoing", state:"CA". Helps track foodborne illness outbreaks and FDA regulations.

Search openFDA Food Enforcement and Recalls database
- **query_medical_devices**: Useful query fields: device.generic_name:"PACEMAKER", event_type:"Malfunction", date_of_event:[20200101 TO 20231231].

Search openFDA Medical Device Adverse Events (MAUDE)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **openFDA** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the most recent food recalls related to Salmonella in California?"

**🤖 AI Agent:**
> I've searched the openFDA Food Enforcement database using the Lucene query `reason_for_recall:"salmonella" AND state:"CA"`. Here are the most recent recall events and associated product descriptions.

---

**👤 You:**
> "Are there any reports of 'insomnia' after taking generic Ibuprofen?"

**🤖 AI Agent:**
> Searching the Drug Adverse Events dataset for `patient.drug.medicinalproduct:"IBUPROFEN" AND patient.reaction.reactionmeddrapt:"INSOMNIA"`. Yes, I've found multiple adverse event records. Here is a summary of the metadata.


## Installation & Usage

To install and use the **openFDA** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openfda](https://vinkius.com/mcp/openfda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
