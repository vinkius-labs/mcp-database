# OpenTHC MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openthc)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Automate cannabis compliance via OpenTHC — track plants, manage inventory, query lab results, and handle B2B/B2C transactions directly from any AI agent.

## Description
Connect your **OpenTHC** Cannabis Regulatory Compliance Engine to any AI agent and take full control of your seed-to-sale workflows through natural conversation.

### What you can do

- **Company & License Management** — List all registered companies and verify active cannabis licenses for compliance assurance
- **Cultivation Tracking** — Query all active plants in cultivation with growth stages, strain varieties, and facility room locations
- **Inventory Control** — Fetch complete inventory ledger including harvested material, work-in-progress, finished goods, and destruction candidates
- **Laboratory Testing** — Access lab samples and Certificates of Analysis (CoA) with full potency, terpene, and contaminant test results
- **B2B Transfers** — Monitor incoming and outgoing wholesale transfer orders with manifests, bills of lading, and fulfillment status
- **Retail Sales** — Retrieve point-of-sale B2C transaction history for daily reporting, tax verification, and purchase limit enforcement
- **Product Catalog** — Browse your complete cannabis product catalog with THC/CBD percentages, SKU data, and regulatory classifications
- **Facility Organization** — List cultivation rooms, processing areas, and operational zones for spatial inventory and workflow planning

### How it works

1. Subscribe to this server
2. Enter your OpenTHC CRE credentials (CRE code, service key, license key, company ID, username, password)
3. Start managing your cannabis compliance from Claude, Cursor, or any MCP-compatible client

No more navigating complex regulatory portals or manually reconciling spreadsheets. Your AI acts as a dedicated compliance officer and operations manager.

### Who is this for?

- **Cultivation Managers** — monitor plant health, predict harvest windows, and ensure plant count limits are respected without opening the CRE portal
- **Compliance Officers** — instantly verify license validity, review lab results, and prepare audit documentation through conversational queries
- **Dispensary Operators** — check product availability, review CoAs before sale, and analyze daily sales patterns directly from the POS system
- **Supply Chain Coordinators** — track B2B transfer status, verify incoming quantities, and orchestrate logistics across licensed facilities


## Available Tools
- **list_b2b_transactions**: Each B2B transaction record contains the transfer ID, direction (incoming/outgoing), counterparty company, transfer status (draft, committed, received, rejected), creation date, expected fulfillment date, line items with quantities, and attached manifests or bills of lading. Essential for supply chain orchestration, logistics planning, and regulatory transfer documentation. AI agents use this to track shipment status, verify received quantities, and prepare compliance reports.

List all B2B transfer transactions (incoming and outgoing)
- **list_b2c_transactions**: Each transaction includes the sale ID, customer information (if recorded), sale date, line items with products and quantities, total amount, tax breakdown, dispensary location, and inventory deduction confirmations. Critical for daily sales reporting, tax calculation verification, inventory reconciliation, and regulatory sales limit enforcement. AI agents should query this to analyze sales patterns, verify compliance with purchase limits, and prepare end-of-day reports.

List all retail B2C sales transactions
- **list_companies**: Use this to understand which organizations are part of your regulatory network, including license holders, cultivators, processors, distributors, and retailers. Each company record contains legal identification data, registration status, and associated license information. Essential for multi-company operations and B2B transaction verification.

List all companies registered in the OpenTHC compliance engine
- **list_contacts**: Each contact includes company affiliation, contact type (B2B partner, regulatory agency, logistics provider), communication details, and relationship status. Use this to identify verified trading partners before creating B2B transfer orders or compliance documentation.

List all business contacts in the OpenTHC network
- **list_inventory**: Each inventory item displays the lot number, item type, quantity with unit of measurement, storage location, creation date, chain of custody history, and compliance status. Fundamental for stock reconciliation, audit preparation, transfer order creation, and regulatory reporting. AI agents should query this before fulfilling orders or conducting inventory audits.

List all inventory items with quantities and locations
- **list_lab_results**: Each result includes the lab result ID, linked sample, testing laboratory accreditation, full analytical results (THC/CBD potency, terpene profile, contaminant levels), pass/fail determination, and the official CoA document reference. Critical for regulatory compliance, product labeling accuracy, retail menu display, and consumer transparency. AI agents should reference this to verify product safety before sale or transfer.

List all laboratory test results and certificates of analysis
- **list_lab_samples**: Each sample contains the sample ID, linked inventory lot, sample type (flower, edible, concentrate), test panel requested (potency, pesticides, heavy metals, mycotoxins, microbials, residual solvents), submission date, testing laboratory, and current analysis status. Essential for quality assurance workflows, batch release decisions, and compliance with mandatory testing regulations. AI agents should check this to determine if a batch has pending or cleared lab results.

List all laboratory samples submitted for testing
- **list_licenses**: Each license contains the license type, expiration dates, regulatory conditions, and approval status. Critical for compliance verification — AI agents should check this before initiating any regulated activity to ensure the proper license is active and valid for the intended operation.

List all cannabis licenses associated with your account
- **list_plants**: Each plant record contains the unique plant ID (POP/PIP tags), growth stage (vegetative, flowering, harvesting), strain/variety, location within the facility (room, rack, shelf), planting date, and estimated harvest window. Critical for cultivation management, compliance reporting, and seed-to-sale traceability. AI agents use this to monitor crop health, predict harvest timelines, and ensure regulatory plant count limits are respected.

List all cannabis plants in active cultivation
- **list_products**: Each product entry contains the product name, type classification, SKU, potency information (THC/CBD percentages), package sizes, and regulatory tags. Essential for retail operations, menu generation, and B2B sales order creation. AI agents should reference this when checking product availability or creating sales transactions.

List all cannabis products in your inventory catalog
- **list_sections**: Each section entry includes the section ID, name, purpose classification (vegetation room, flowering room, drying room, processing area, retail floor, warehouse), environmental parameters, and capacity limits. Essential for spatial inventory tracking, cultivation workflow organization, facility compliance inspections, and operational planning. AI agents use this to assign plants to specific rooms during cultivation activities, locate inventory within the facility, and generate room-level production reports.

List all facility sections and cultivation areas
- **list_varieties**: Each variety record contains the variety ID, strain name (e.g., Blue Dream, OG Kush, Sour Diesel), genetics type (Type I - THC dominant, Type II - Mixed THC/CBD, Type III - CBD dominant), breeder information, and associated cultivation characteristics. Fundamental for cultivation planning, product labeling, genetic tracking, and regulatory strain registration. AI agents reference this when creating new plant records, generating product labels, or analyzing strain performance metrics.

List all cannabis varieties (strains) in the system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenTHC** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our active cannabis licenses and verify which ones are expiring soon."

**🤖 AI Agent:**
> I've fetched your regulatory licenses. You currently hold 3 active licenses: Cultivation License #CU-2024-0891 (expires 2026-12-31), Processing License #PR-2024-0345 (expires 2025-06-30 — expiring in 89 days), and Retail License #RT-2024-1122 (expires 2027-03-15). Would you like me to prepare a renewal checklist for the Processing license?

---

**👤 You:**
> "Show me all plants currently in flowering stage in Room 3 and estimate harvest readiness."

**🤖 AI Agent:**
> Running cultivation query... I found 127 active plants in Room 3 (Flowering Chamber). Breakdown: 85 Blue Dream plants (Week 6 of 8 flowering — harvest estimated 2025-04-21), 42 OG Kush plants (Week 4 of 9 — harvest estimated 2025-05-05). All plants are within compliance plant count limits. Environmental logs show optimal conditions. Would you like nutrient schedules or trimming crew assignments for the upcoming Blue Dream harvest?

---

**👤 You:**
> "Check inventory levels for all THC-dominant flower products and show me pending lab results."

**🤖 AI Agent:**
> Cross-referencing inventory and lab testing... Current THC flower stock: 14.2 kg of Blue Dream (Lot BD-2025-0412), 8.7 kg OG Kush (Lot OG-2025-0398), and 3.1 kg Sour Diesel (Lot SD-2025-0445). Pending lab results: 2 batches awaiting clearance — Lot BD-2025-0419 (potency panel, results expected 2025-04-10) and Lot OG-2025-0421 (full pesticide panel, results expected 2025-04-12). All currently available stock has valid CoAs. Should I flag any inventory nearing expiration?


## ❓ FAQ

**Q: Can my AI automatically check if a cannabis batch has passed laboratory testing before I approve a sale?**
Yes! Use the `list_lab_results` tool to fetch all Certificates of Analysis (CoA) and review potency, terpene profiles, and contaminant test results. Your AI agent will respond with complete pass/fail determinations and analytical data linked to specific inventory lots. Always verify CoA clearance before creating B2B transfer orders or retail sales to ensure regulatory compliance.

**Q: How do I quickly list all active plants in a specific cultivation room to check growth stages and predict harvest windows?**
Simply ask the agent to run the `list_plants` action. It will compile all active plant records with their POP/PIP tags, current growth stage (vegetative, flowering, harvesting), strain variety, and estimated harvest dates. For facility-specific filtering, cross-reference with the `list_sections` tool to identify the target cultivation room GID and request plants assigned to that spatial zone.

**Q: Does the OpenTHC integration permit modifying or destroying inventory records?**
No. The current tool set focuses strictly on read-only querying and analytical operations — listing companies, verifying licenses, inspecting inventory, reviewing lab results, and tracking B2B/B2C transactions. State alteration operations (creating, adjusting, or destroying inventory) are not currently exposed, assuring your compliance records remain secure against destructive queries. This design prioritizes audit readiness and regulatory reporting safety.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openthc](https://vinkius.com/mcp/openthc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenTHC** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `openthc` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenTHC** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openthc": {
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
