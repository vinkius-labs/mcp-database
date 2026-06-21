# OpenFDA MCP Server

Access FDA drug safety data, device recalls, food enforcement reports and approved drug information.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/openfda-alternative)

## Overview
**Category:** the-unthinkable
**Tools Count:** 8

## Description
Connect to **OpenFDA** and explore the FDA's open data platform through natural conversation — no API key needed.

### What you can do

- **Drug Adverse Events** — Search the FDA Adverse Event Reporting System (FAERS) for drug safety reports
- **Device Adverse Events** — Search medical device malfunction and injury reports (MAUDE database)
- **Food Recalls** — Find food product recall enforcement reports with classification and distribution info
- **Drug Labels** — Search structured drug labeling data with ingredients, warnings and dosage info
- **Approved Drugs** — Search Drugs@FDA for approved drug applications with sponsor and approval details
- **Device Recalls** — Find medical device recall enforcement reports
- **Device Clearance** — Search 510(k) premarket device clearance data
- **Animal & Veterinary** — Search adverse event reports for animal drugs and veterinary products

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Explore FDA safety data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Healthcare Professionals** — monitor drug safety signals, device malfunctions and recall notifications
- **Researchers** — analyze adverse event patterns, drug safety trends and device performance
- **Patients** — find information about drug side effects, device recalls and food safety alerts


## Available Tools
- **search_animal_events**: Returns reports of adverse events in animals from drug exposure. Use search syntax: animal.species="dog" or drug.active_ingredient="ivermectin".

Search animal and veterinary adverse event reports
- **search_device_clearance**: Returns device names, 510(k) numbers, applicant names, decision dates, regulation numbers and product codes.

Search 510(k) premarket device clearance data
- **search_device_events**: Returns reports of device malfunctions, injuries and deaths. Use search syntax: device.brand_name="pacemaker" or patient.problems.problem_text="infection".

Search medical device adverse event reports
- **search_device_recalls**: Returns recalled devices with reason for recall, classification, recalling firm, product description, code_info and distribution pattern.

Search medical device recall reports
- **search_drugsfda**: Returns drug names, active ingredients, application numbers, sponsors/manufacturers, approval dates and product details. Use search syntax: openfda.brand_name:"Lipitor" or openfda.generic_name:"atorvastatin".

Search FDA-approved drug applications
- **search_drug_events**: Returns adverse events submitted by healthcare professionals, consumers and manufacturers. Use search syntax: patient.reaction.reactionmeddrapt="headache" or openfda.brand_name="Advil". Supports pagination with limit (max 1000) and skip parameters.

Search drug adverse event reports
- **search_drug_labels**: Returns drug labels with active ingredients, purpose, warnings, dosage, indications, manufacturer info and more. Use search syntax: openfda.brand_name:"Advil" or effective_time:"2024".

Search drug labeling information
- **search_food_recalls**: Returns recalled food products with reason for recall, classification (Class I/II/III), recalling firm, distribution and product description.

Search food recall enforcement reports


## Installation & Usage

To install and use the **OpenFDA** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openfda-alternative](https://vinkius.com/mcp/openfda-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
