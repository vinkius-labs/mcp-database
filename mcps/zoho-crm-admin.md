# Zoho CRM Admin MCP Server

Manage Zoho CRM users, roles, profiles, layouts, territories, and tags — complete admin control through conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-crm-admin)

## Overview
**Category:** industry-titans
**Tools Count:** 7

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
- **zoho_get_user**: Returns full profile: name, email, role, profile (permissions), locale, timezone, created date, and last activity. Use to get detailed info about a specific team member or administrator.

Get complete details of a specific Zoho CRM user by ID, including role, profile, locale, and activity info
- **zoho_list_layouts**: Returns layout name, status (active/inactive), and section structure. Layouts define how the record form appears in the UI — which fields are shown, their grouping into sections, and display order. Different layouts can be assigned to different profiles. Use when the user asks about form configuration or field arrangement.

List page layouts for a Zoho CRM module, showing the form structure with sections and field arrangement
- **zoho_list_profiles**: Returns profile name, description, and whether it is the default. Profiles are permission sets controlling module access, field-level visibility, and feature availability (e.g., Administrator, Standard, Marketing). While roles control data visibility, profiles control feature access. Use to audit permissions or understand what different user groups can do.

List Zoho CRM profiles (permission sets) that control what features, modules, and actions users can access
- **zoho_list_roles**: Returns role name, reporting role (parent in the hierarchy), and description. Roles control data visibility — users can see records of their subordinate roles. Use to understand the organizational hierarchy, access control structure, or when the user asks about role assignments.

List all roles in Zoho CRM with their hierarchy structure, showing who reports to whom in the organization
- **zoho_list_tags**: Returns tag name, color, and creator. Tags are user-defined labels for quick categorization and filtering of records (e.g., "VIP", "Urgent", "Follow-up Required"). Use when the user asks about available tags, wants to understand how records are categorized, or needs tag names for filtering.

List all tags available for a Zoho CRM module for record categorization and quick filtering
- **zoho_list_territories**: Returns territory name, manager, parent territory, and description. Territories organize the sales team by geography, product line, or customer segment (e.g., "North America", "Enterprise", "EMEA"). Records can be assigned to territories for routing and reporting. Use when the user asks about sales territories or geographic coverage.

List sales territories in Zoho CRM with territory names, managers, and hierarchy for geographic/segment-based sales organization
- **zoho_list_users**: Returns user name, email, role, profile (permission set), active/inactive status, and timezone. Filter by type: AllUsers, ActiveUsers, DeactiveUsers, AdminUsers. Use when the user asks about team members, needs user IDs for record assignment, or wants to audit CRM access.

List Zoho CRM users with name, email, role, profile, status, and timezone for team management visibility


## Installation & Usage

To install and use the **Zoho CRM Admin** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-crm-admin](https://vinkius.com/mcp/zoho-crm-admin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
