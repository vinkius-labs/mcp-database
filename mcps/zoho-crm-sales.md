# Zoho CRM Sales MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-crm-sales)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zoho-crm-sales-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zoho-crm-sales-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Deep deal management with quotes, products, sales orders, and invoices — complete sales cycle in Zoho CRM.

## Description
Connect **Zoho CRM** to any AI agent — manage your entire CRM without switching tabs.

### What you can do
- **Leads** — Search and create leads with source and status tracking
- **Contacts** — Find and create contacts linked to accounts
- **Accounts** — Search companies and organizations
- **Deals** — Search, create, and track deals through pipeline stages
- **Notes** — Create notes attached to any CRM record
- **Generic List** — Query any Zoho CRM module directly

### Who is this for?
- **Sales Reps** — CRM at your fingertips through AI
- **BDRs** — Quickly qualify and create leads
- **Sales Managers** — Pipeline visibility and deal insights
- **Support Teams** — Access contact and account data seamlessly


## Available Tools
- **zoho_create_deal**: Deal_Name is required. Stages: Qualification, Needs Analysis, Value Proposition, Proposal/Price Quote, Negotiation/Review, Closed Won, Closed Lost. Pipeline lets you assign to a specific sales pipeline (if multiple exist). Closing_Date is YYYY-MM-DD.

Create a new deal/opportunity in Zoho CRM with name, stage, amount, pipeline, and closing date
- **zoho_create_product**: Product_Name is required. Unit_Price is the default price. Product_Code serves as the SKU/identifier. Products can be added to quotes and sales orders. Returns the created product with its Zoho ID.

Create a new product in the Zoho CRM catalog with name, unit price, product code, and description
- **zoho_create_quote**: Subject is required. Link to a deal via Deal_Name and an account via Account_Name. Valid_Till sets the expiration date (YYYY-MM-DD). Line items/products should be added separately via the Zoho UI. Returns the created quote with its ID.

Create a sales quote in Zoho CRM linked to a deal and account with subject, validity, and pricing
- **zoho_get_deal**: Returns full deal data: name, stage, amount, probability, closing date, account, contact, and custom fields. Use after searching to drill into a specific opportunity.

Get complete details of a specific Zoho CRM deal by ID, including all custom fields, notes, and history
- **zoho_list_invoices**: Invoices are billing documents generated from sales orders or deals. Returns subject, status, account, total, due date, and whether payment is received. Use when the user asks about billing, outstanding invoices, or payment tracking.

List invoices in Zoho CRM with subject, status, account, total amount, due date, and payment status
- **zoho_list_quotes**: Quotes are formal price proposals created for deals. Returns subject, total, linked deal and account, valid until date, and status. Use when the user asks about pending quotes, proposal status, or pricing documents.

List sales quotes in Zoho CRM with subject, quoted amount, account, validity period, and status
- **zoho_list_sales_orders**: Sales orders are confirmed purchase commitments from customers, created after quote approval. Returns subject, status, account, total, and expected ship date. Use when the user asks about confirmed orders or fulfillment pipeline.

List sales orders in Zoho CRM with subject, status, account, total amount, and fulfillment details
- **zoho_search_deals**: Returns deal name, pipeline stage (Qualification/Needs Analysis/Proposal/Negotiation/Closed Won/Closed Lost), amount, closing date, and linked account. Use when the user asks about pipeline status, specific deal values, or opportunity progress.

Search Zoho CRM deals by name to find active sales opportunities with stage, amount, account, and closing date
- **zoho_search_products**: Returns product name, unit price, product code (SKU), and description. Products are catalog items that can be attached to quotes, sales orders, and invoices. Use when looking up product details or pricing.

Search the Zoho CRM product catalog by name to find items with prices, codes, and descriptions
- **zoho_update_deal**: Only specified fields change. Common operations: advance Stage when deal progresses, update Amount after negotiation, push Closing_Date when timeline shifts, or set Stage to "Closed Won"/"Closed Lost" to close.

Update an existing Zoho CRM deal — advance stage, change amount, or update closing date to reflect pipeline progress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho CRM Sales** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for leads from web form"

**🤖 AI Agent:**
> 👥 **Leads from Web Form**
| Name | Email | Company | Status |
|---|---|---|---|
| John Smith | john@acme.com | Acme Corp | New |
| Maria Garcia | maria@beta.io | Beta Inc | Contacted |

---

**👤 You:**
> "Create a deal: Enterprise Plan $25,000"

**🤖 AI Agent:**
> ✅ **Deal Created!**
- Name: Enterprise Plan
- Amount: $25,000
- Stage: Qualification
- Closing: 2024-03-30


## Installation & Usage

To install and use the **Zoho CRM Sales** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-crm-sales](https://vinkius.com/mcp/zoho-crm-sales)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
