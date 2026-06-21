# openFDA MCP Server

Access the powerful openFDA databases for drug adverse events, food recalls, and medical device safety reports globally.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/openfda)

## Overview
**Category:** the-unthinkable
**Tools Count:** 3

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


## Installation & Usage

To install and use the **openFDA** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openfda](https://vinkius.com/mcp/openfda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
