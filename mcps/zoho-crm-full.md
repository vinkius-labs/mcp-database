# Zoho CRM (Full) MCP Server

Manage leads, contacts, accounts, deals, and notes — complete Zoho CRM access through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-crm-full)

## Overview
**Category:** productivity
**Tools Count:** 9

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
- **zoho_create_contact**: Last_Name is required. Account_Name links the contact to an existing account (company). Contacts represent qualified individuals in the CRM — use for customers, partners, or qualified prospects.

Create a new contact in Zoho CRM with name, email, phone, and linked account for customer management
- **zoho_create_deal**: Deal_Name is required. Stages: Qualification, Needs Analysis, Value Proposition, Identify Decision Makers, Proposal/Price Quote, Negotiation/Review, Closed Won, Closed Lost. Amount is numeric. Closing_Date uses YYYY-MM-DD. Account_Name links to an existing account.

Create a new deal/opportunity in Zoho CRM with name, stage, amount, closing date, and linked account
- **zoho_create_lead**: Last_Name is required. Lead_Source values: Web Download, Advertisement, Cold Call, Employee Referral, External Referral, Partner, Conference, Trade Show. Lead_Status values: Not Contacted, Contacted, Contact in Future, Junk Lead, Lost Lead. Returns the created lead with its Zoho ID.

Create a new lead in Zoho CRM with name, email, company, phone, source, and status for pipeline entry
- **zoho_create_note**: Note_Title and Note_Content are required. Link to a parent by providing Parent_Id and se_module (Leads, Contacts, Deals, Accounts). Notes appear in the record timeline. Use to log meeting summaries, call notes, or internal context.

Create a note in Zoho CRM attached to a lead, contact, deal, or account for activity logging and history
- **zoho_list_records**: Module names: Leads, Contacts, Accounts, Deals, Tasks, Events, Calls, Notes, Products, Quotes, Sales_Orders, Invoices, Purchase_Orders. Returns records sorted by modification date. Use when the user wants to browse recent records or get a general overview of a module.

List recent records from any Zoho CRM module (Leads, Contacts, Accounts, Deals, Tasks, etc.) for browsing
- **zoho_search_accounts**: Returns account name, industry, website, phone, annual revenue, and owner. Accounts are the company-level records that contacts and deals are linked to. Use when the user asks about a company, needs account-level data, or wants to find an account ID.

Search Zoho CRM accounts (companies/organizations) by name to find business entities in your CRM
- **zoho_search_contacts**: Returns contact name, email, phone, linked account, and owner. Contacts differ from Leads — they are qualified prospects that have been converted or manually entered. Use when the user asks about a customer or needs contact details.

Search Zoho CRM contacts by name or email to find converted prospects and existing customers
- **zoho_search_deals**: Returns deal name, stage (e.g., Qualification, Needs Analysis, Proposal, Negotiation, Closed Won/Lost), amount, closing date, and linked account. Use when the user asks about pipeline opportunities, deal values, or wants to check deal progress.

Search Zoho CRM deals by name to find sales opportunities with stage, amount, and closing date
- **zoho_search_leads**: Returns lead name, email, company, lead source (Web, Advertisement, Referral, etc.), lead status (Not Contacted, Contacted, Junk Lead, etc.), and owner. Use when the user wants to find a potential customer, check lead status, or review the top of the sales funnel.

Search Zoho CRM leads by name, email, or company to find prospective customers in the sales funnel


## Installation & Usage

To install and use the **Zoho CRM (Full)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-crm-full](https://vinkius.com/mcp/zoho-crm-full)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
