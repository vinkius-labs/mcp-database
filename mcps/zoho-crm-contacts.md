# Zoho CRM Contacts MCP Server

Search, create, and manage contacts, leads, and accounts — with lead conversion and related records in Zoho CRM.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-crm-contacts)

## Overview
**Category:** sales-automation
**Tools Count:** 11

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
- **zoho_convert_lead**: This is the standard sales qualification workflow in Zoho CRM. The lead is removed from the Leads module and data transfers to the new records. Use when a lead is qualified and ready to enter the sales pipeline.

Convert a qualified Zoho CRM lead into a Contact + Account + Deal — the key sales qualification step
- **zoho_create_account**: Account_Name is required. Industry should match Zoho industry picklist values. Once created, contacts and deals can be linked to this account.

Create a new account (company/organization) in Zoho CRM with name, industry, phone, and website
- **zoho_create_contact**: Last_Name is required. Account_Name links the contact to a company account. Use for adding qualified individuals — not raw leads (use zoho_create_lead for unqualified prospects).

Create a new contact in Zoho CRM with name, email, phone, and linked account for customer management
- **zoho_create_lead**: Last_Name is required. Use for new, unqualified prospects. Lead_Source: Web Download, Advertisement, Cold Call, Employee Referral, External Referral, Partner, Conference, Trade Show. Once qualified, convert using zoho_convert_lead.

Create a new lead (unqualified prospect) in Zoho CRM with name, email, company, and lead source
- **zoho_get_account**: Returns account name, industry, annual revenue, employees, billing/shipping address, and all custom fields. Use after searching to get full company details.

Get complete details of a specific Zoho CRM account by ID, including industry, revenue, and linked records
- **zoho_get_contact**: Returns full data: name, emails, phones, account, department, title, mailing address, and custom fields. Use after searching to drill into contact details.

Get complete details of a specific Zoho CRM contact by ID, including all custom fields and linked records
- **zoho_related_records**: For example: module="Accounts", recordId="123", relatedModule="Contacts" returns all contacts at that account. Common patterns: Accounts→Contacts, Contacts→Deals, Deals→Notes, Accounts→Deals. Use when the user asks "who are the contacts at this company?" or "what deals does this contact have?"

Get records related to a parent record in Zoho CRM — e.g., contacts of an account, deals of a contact, notes of a lead
- **zoho_search_accounts**: Returns account name, industry, website, phone, annual revenue, and owner. Accounts are the company-level records that contacts and deals are linked to.

Search Zoho CRM accounts (companies) by name to find business entities and their organizational data
- **zoho_search_contacts**: Returns contact name, email, phone, linked account, and owner. Contacts represent qualified individuals — converted leads or manually created customer records. Use when the user asks about a specific person or needs contact details.

Search Zoho CRM contacts by name or email to find qualified prospects and existing customers
- **zoho_search_leads**: Returns lead name, email, company, lead source (Web/Advertisement/Referral), lead status (Not Contacted/Contacted/Junk), and owner. Leads are the top-of-funnel — unqualified prospects. Once qualified, they can be converted to contacts+accounts+deals.

Search Zoho CRM leads by name, email, or company to find unqualified prospects at the top of the funnel
- **zoho_update_contact**: Only specified fields change. Use to correct info, update phone numbers, or reassign accounts.

Update an existing Zoho CRM contact — change name, email, phone, or other properties


## Installation & Usage

To install and use the **Zoho CRM Contacts** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-crm-contacts](https://vinkius.com/mcp/zoho-crm-contacts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
